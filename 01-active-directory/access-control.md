# Department-Based Access Control

## Objective

The objective of this lab was to implement department-based access control so that employees can access only the files required for their role.

The environment uses Active Directory security groups combined with NTFS permissions on a Windows Server file share.

---

## Lab Environment

- Operating System: Windows Server 2025
- Client: Windows 11
- Domain: `lab.local`
- Domain Controller: `WIN-SRV01`
- File server directory: `C:\CompanyData`
- File sharing protocol: SMB

---

## File Server Structure

A central company data directory was created on the Windows Server:

```text
C:\CompanyData
├── HR
├── IT
└── Management
