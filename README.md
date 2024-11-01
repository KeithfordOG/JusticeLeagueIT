# 🚀 Justice League Device Management Project 🌌

This project configures and manages devices for the Justice League team using **Microsoft Intune**. The setup includes device compliance policies, configuration profiles, and role-based access, ensuring each hero has secure and appropriate access to resources. 🦸‍♂️🦸‍♀️

---

## 📑 Table of Contents

1. [🌟 Overview](#overview)
2. [🛠️ Setup Steps](#setup-steps)
   - [1. Users and Groups Setup](#1-users-and-groups-setup)
   - [2. Assign Intune Roles and Scope Groups](#2-assign-intune-roles-and-scope-groups)
   - [3. Compliance Policies](#3-compliance-policies)
   - [4. Configuration Profiles](#4-configuration-profiles)
   - [5. Monitoring and Management](#6-monitoring-and-management)
3. [📂 Project Structure](#project-structure)


---

## 🌟 Overview

The **Justice League Device Management Project** sets up and enforces security and compliance policies across different platforms (iOS, Android, Windows) using Microsoft Intune. This project includes:

- 🔒 **Role-based access control** for different responsibilities (Admin, Help Desk, Profile/Policy Manager, Read Only).
- 🛡️ **Compliance policies** for device health and security.
- ⚙️ **Configuration profiles** for device settings like Wi-Fi, VPN, and app restrictions.


---

## 🛠️ Setup Steps

### 1. 👥 Users and Groups Setup

- **Create Users**: In the Microsoft 365 Admin Center, create accounts for Justice League members (e.g., Batman, Wonder Woman). Assign Intune licenses to each.
  ![Creating Users](Images/users.png)

- **Create Role-Based Groups**:
  - 👑 Admin
  - 🛠️ Help Desk
  - 📄 Profile/Policy Manager
  - 👀 Read Only
    ![Creating Security Groups](Images/groups.png)
- **Add Members**: Assign each member to the appropriate group based on their heroic responsibilities.

### 2. 🎛️ Assign Intune Roles and Scope Groups

- **Assign Intune Roles**: In Microsoft Endpoint Manager, assign each role to its corresponding group (e.g., Help Desk Operator role to the Help Desk group).
- **Set Scope Groups**: Define which devices or users each role can manage by assigning scope groups (e.g., assign Profile/Policy Manager to manage iOS devices only).

### 3. ✅ Compliance Policies

- **iOS Compliance Policy**:
  - 📱 Settings include password requirements, encryption, and blocking jailbroken devices.
  - 🚨 Assign the policy to all iOS device groups (e.g., All iOS Devices or Justice League Members).
 ![Creating Compliance Policy](Images/compliancepolicy.png)

### 4. 🔧 Configuration Profiles

- **Create iOS Configuration Profile**:
  - Use the **Settings Catalog** or **Templates** for device restrictions, Wi-Fi, or VPN.
  - 🔐 Settings include password requirements, network restrictions, and app permissions.
  - 📋 Assign this profile to all iOS device groups.



### 5. 📊 Monitoring and Management

- **Monitor Compliance**: In Endpoint Manager, go to **Reports** > **Device Compliance** to view device compliance status.
- **Testing**: Enroll a test device to validate compliance and configuration settings.
   ![Monitoring Compliance](Images/monitor.png)

---



