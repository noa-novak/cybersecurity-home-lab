# Active Directory Domain Setup

## Objective

The objective of this stage was to create a Windows Server 2025 Active Directory environment for a simulated small company.

## Lab Environment

- Host OS: Fedora Linux
- Virtualization: Virtual Machine Manager
- Server OS: Windows Server 2025
- Client OS: Windows 11
- Domain: `lab.local`
- Domain Controller: `WIN-SRV01`

## Implementation

Windows Server 2025 was configured as an Active Directory Domain Controller.

The server provides:

- Active Directory Domain Services (AD DS)
- DNS
- Domain authentication
- Centralized user and group management

A Windows 11 virtual machine was joined to the `lab.local` domain and used as the domain client.

## Domain Structure

The following organizational units were created:

- HR
- IT
- Management
- Groups

The organizational units are used to organize users and security objects within the domain.

## Verification

The Windows 11 client was successfully joined to the `lab.local` domain.

Domain users were able to authenticate on the Windows 11 client using their Active Directory credentials.

## Result

The basic Active Directory infrastructure is operational and provides centralized authentication and identity management for the lab.
