# BMT-Windows-Server-Lab

## Overview

A home lab simulating the IT infrastructure of a fictional company called Blue Mountain Technologies. The lab is configured with a virtualized domain controller, Active Directory, organizational units, multiple user accounts, security groups, Group Policy configurations, and drive mapped department-based file shares.

## Environment

- Windows Server 2022 Domain Controller
- Windows 11 Workstation
- Oracle VirtualBox
- Active Directory Domain Services
- DNS/DHCP
- Group Policy
- SMB File Sharing

## Implemented

- Created Active Directory OUs for Finance and HR departments
- Created user accounts and security groups
- Configured Group Policy Objects to implement security settings and automatic drive mapping
- Created SMB file shares based on the departments
- Configured NTFS and share permissions
- Tested access control between departments

## Active Directory

Configured Active Directory complete with OUs for User and Computer Departments and Security Groups.
<img width="1390" height="1069" alt="AD Finance Users OU" src="https://github.com/user-attachments/assets/786b757b-085c-4fe5-8f34-30013a30d938" />
<img width="1390" height="1071" alt="AD HR Workstations OU" src="https://github.com/user-attachments/assets/018c912e-9b62-4e61-9e10-81958a25ab70" />
<img width="1394" height="1070" alt="AD Security Groups" src="https://github.com/user-attachments/assets/9c006634-b5ed-4d65-b375-cc641c0f3150" />

## Group Policy

Created and configured department specific policies and applied them to the proper OUs.
<img width="1391" height="1072" alt="Group Policy Objects" src="https://github.com/user-attachments/assets/d65c8bbd-50ce-4dc4-bc36-eeb2a461b65a" />
<img width="1391" height="1071" alt="HR Group Policy Drive Mapping" src="https://github.com/user-attachments/assets/4b5c0427-17a4-4d29-8fc9-ba1e30a99c49" />
<img width="1390" height="1068" alt="Finance Group Policy Drive Mapping" src="https://github.com/user-attachments/assets/3421544c-a6e6-4c23-ac20-92374058c0c6" />

## File Shares

Configured accurate drive mapping to automatically map drives to the correct users. Mapped the H: drive to the HR users and the F: Drive to the Finance users.
<img width="1395" height="1070" alt="SMB Shares and File Paths" src="https://github.com/user-attachments/assets/fa0edfda-b817-4a5b-aa08-0974d073c073" />

## Access Control Testing

HR users successfully accessed HR files and Finance users were denied access.
<img width="1020" height="847" alt="HR files accessed by HR User" src="https://github.com/user-attachments/assets/9bb11feb-974a-4710-baad-50cba16422b9" />
<img width="1022" height="846" alt="HR Folder Access Denied to Finance User" src="https://github.com/user-attachments/assets/5b26c633-93e3-44f0-acfd-e0e3ea6ae34b" />

Finance users successfully accessed Finance Files while HR users were denied access.
<img width="1021" height="848" alt="Finance Files Accessed by Finance User" src="https://github.com/user-attachments/assets/1d832de9-f47b-48d1-b3e8-3a4c55d794fa" />
<img width="1019" height="847" alt="Access to Finance Files Denied" src="https://github.com/user-attachments/assets/ea76a690-65f1-4ddc-9fce-60a1d4415d01" />




