

## 🛡️ Group Policy Management Home Lab: Creating and Setting Up GPOs

Welcome to my **Group Policy Management (GPO)** home lab. This lab demonstrates how to install and configure Group Policy Objects in a Windows Server environment to enforce security standards and administrative controls across a domain.

It walks through every key step—from understanding GPO concepts to installing tools, creating policies, and applying them. By the end, you'll see how I use this setup to manage and secure enterprise environments.

---

### 🧠 What is GPO?

**Group Policy Object (GPO)** is a feature of Microsoft Windows Active Directory that provides centralized management and configuration of operating systems, applications, and users' settings.

GPOs allow administrators to:

* Enforce password policies
* Configure desktop environments
* Install software
* Set user rights
* Restrict access to certain features or areas

---

### ✅ Prerequisites

Before starting this lab, make sure you have:

* A functioning **Windows Server** VM with **Active Directory Domain Services (AD DS)** installed
* A **domain-joined Windows 10/11 client**
* Admin privileges on the domain controller
* Basic understanding of Active Directory and Windows Server roles

---

### 📚 GPO Review

This section offers a quick theoretical review of Group Policy concepts:

* **Local GPO**: Applies settings to the local machine
* **Non-local GPO**: Created in AD DS and applies to users/computers in OUs
* **Group Policy Inheritance**: Policies are inherited from parent OUs unless blocked
* **Policy Precedence**: Local < Site < Domain < OU

GPO settings are divided into:

* **Computer Configuration**: Applied during system startup
* **User Configuration**: Applied at user login

---

### 🛠️ Installing the Group Policy Management Console (GPMC)

To manage GPOs, the **GPMC** must be installed.

#### Steps:

1. On the domain controller:

   * Open **Server Manager**
   * Click **Add Roles and Features**
   * Select **Group Policy Management**
   * Finish installation

2. Open GPMC via:

   ```
   Start > Administrative Tools > Group Policy Management
   ```

---

### 🧪 Creating GPOs + Types of GPOs

There are multiple ways to create and assign GPOs. Below are the steps and types.

#### How to Create a GPO:

1. Open **Group Policy Management**
2. Right-click on the **OU or Domain** where you want to apply the GPO
3. Select **Create a GPO in this domain, and Link it here**
4. Name your GPO (e.g., *PasswordPolicy-GPO*)
5. Right-click the GPO and choose **Edit**
6. Configure settings under **Computer Configuration** or **User Configuration**

#### Types of GPOs:

| Type            | Description                                                 |
| --------------- | ----------------------------------------------------------- |
| **Local GPO**   | Applies only to local machines                              |
| **Domain GPO**  | Managed centrally via AD DS                                 |
| **Starter GPO** | Template GPO used to create new GPOs with baseline settings |
| **Linked GPO**  | GPOs linked to Sites, Domains, or OUs                       |

---

### 🧩 Example GPO Scenarios


* Enforcing password length
* Locking the desktop after inactivity
* Preventing access to Control Panel
* Configuring Windows Update behavior

---

### 🧾 Conclusion: Why This Lab?

This lab highlights my capability to:

* Build and configure a fully functional Windows Server lab environment
* Understand and apply Group Policy to enforce enterprise security controls
* Document and automate configuration management

**It demonstrates my foundational skills in system administration, security policy enforcement, and enterprise IT management.**

---


