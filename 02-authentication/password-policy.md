# Domain Password Policy

## Objective

The objective was to strengthen authentication security by implementing a domain-wide password policy.

## Configuration

The Active Directory default domain password policy was configured with the following settings:

| Setting | Value |
|---|---:|
| Minimum password length | 12 characters |
| Password history | 5 passwords |
| Password complexity | Enabled |
| Maximum password age | 90 days |
| Minimum password age | 1 day |
| Account lockout threshold | 5 failed attempts |
| Lockout duration | 15 minutes |
| Observation window | 15 minutes |

## Implementation

The domain password policy was configured using PowerShell.

The configuration was verified using:

```powershell
Get-ADDefaultDomainPasswordPolicy -Identity "lab.local" |
Format-List
