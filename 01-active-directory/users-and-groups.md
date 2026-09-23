# Active Directory Users and Groups

## Objective

The objective was to create a realistic department-based Active Directory structure using users, organizational units, and security groups.

## Users

The following domain users were created:

| User | Department | Security Group |
|---|---|---|
| Sarah Weber | HR | HR-Users |
| Max Mueller | IT | IT-Users |
| John Schmidt | Management | Management |

## Organizational Units

Users were organized into department-specific organizational units:

- HR
- IT
- Management

A separate `Groups` OU was created for security groups.

## Security Groups

The following security groups were created:

- `HR-Users`
- `IT-Users`
- `Management`

Security groups were used instead of assigning file permissions directly to individual users.

## Why Groups Were Used

Using security groups makes access management easier to maintain.

For example, if another employee joins the HR department, the administrator only needs to add the employee to `HR-Users`. The existing permissions can then apply automatically.

This follows the principle of managing permissions through groups rather than individual accounts.

## Verification

Group membership was verified using PowerShell:

```powershell
Get-ADGroupMember "HR-Users"
Get-ADGroupMember "IT-Users"
Get-ADGroupMember "Management"
