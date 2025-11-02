<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket Post Install and Setup
This project demonstrates how I deployed and configured the open-source osTicket help desk ticketing system on a Windows 11 virtual machine hosted in Microsoft Azure.
The goal of this lab was to practice configuring key administrative components within osTicket — including Roles, Departments, Teams, Agents, Users, SLAs, and Help Topics — to simulate a functional IT support environment.
This lab builds upon my previous osTicket Setup repository and continues the process of creating a complete end-to-end help desk system deployment.
<br />

# Skills Demonstrated
- Cloud Computing: Provisioned and managed a Microsoft Azure virtual machine
- Web Server Administration: Configured IIS for PHP and MySQL integration
- Application Deployment: Installed and deployed the osTicket help desk system
- System Configuration: Managed Roles, Agents, Users, and Teams within osTicket
- Policy Management: Created SLAs (Service Level Agreements) and Help Topics to define ticket workflows
- Platform Navigation: Operated both the Admin Panel and Agent Panel for end-to-end system functionality

# Prerequisites
- <a href="https://azure.microsoft.com/en-us"> Microsoft Azure (Virtual Machines/Compute)
- <a href="https://support.microsoft.com/en-us/windows/how-to-use-remote-desktop-5fe128d5-8fb1-7a23-3b8a-41e636865e8c"> Remote Desktop
- Internet Information Services (IIS)
- Windows 11 Pro (24H2)
- PHP 7.3.8
- MySQL 5.5.62
- HeidiSQL
- PHP Manager for IIS
- Rewrite Module for IIS

# Deployment and Phases Overview
- Below are the main steps (Phases 1-22) I followed to fully deploy osTicket.
  # Deployment and Phases

## Phase 1
  - In osTicket Configure Roles (for grouping permissions
  - Admin Panel -> Agents -> Roles -> Supreme Admin -> check every perm
  - 
<img width="800" height="800" alt="Post Install Phase 1" src="https://github.com/user-attachments/assets/6ac4335a-56b4-4481-80bd-097924c06692" />

## Phase 2
  - in osTicket Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
  - Admin Panel -> Agents -> Departments -> Name Sys Admin
  
<img width="800" height="800" alt="Post Install Phase 2" src="https://github.com/user-attachments/assets/86202821-e6e2-4d79-a600-2f92005ea677" />

## Phase 3
  - in osTicket Configure Teams
  - Admin Panel -> Agents -> Teams(Pull Agents from different Departments) -> Online Banking

<img width="800" height="800" alt="Post Instal Phase 3" src="https://github.com/user-attachments/assets/37aab3f2-3121-4d32-aad7-37c99120092a" />

## Phase 4
  - Allow anyone to create tickets
  - Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets) -> Registration Required: Require Registration and login to create tickets

<img width="800" height="800" alt="Post Intall Phase 4" src="https://github.com/user-attachments/assets/9a766f63-159f-4249-b67a-5cf7a2f9e3b5" />

## Phase 5
  - in osTicket Configure Agents (workers)
  - Admin Panel -> Agents -> Add New -> Jane Doe (Dept: Sys Admin) and -> John Doe (Dept: Support)
  - Also set a password for both jane and john make sure require password change box is unchecked
<img width="800" height="800" alt="Screenshot 2025-11-01 091014" src="https://github.com/user-attachments/assets/f91bd61c-5498-425e-a751-05e4057d5be7" />
<img width="800" height="800" alt="Screenshot 2025-11-01 091112" src="https://github.com/user-attachments/assets/7841ea9b-cb4e-4c0c-abcc-8971899eca00" />
<img width="2559" height="1439" alt="Screenshot 2025-11-01 091503" src="https://github.com/user-attachments/assets/d398685b-d2a3-4647-96ba-51e13e10db52" />





    
