# Azure vs AWS vs Google Cloud: Identity and Access Management (IAM)

## Azure Microsoft Entra ID (Azure Active Directory)

### 1. What is Microsoft Entra ID?

![image](https://github.com/user-attachments/assets/5b1bfa29-85c9-4da2-989e-7c25f7cfa6e8)

**Microsoft Entra ID** is Microsoft’s cloud-based **Identity(Authentication) and Access Management(Authorization)** IAM service. It helps employees, partners, and customers securely access resources such as:

- Microsoft 365

- Azure

- Applications (SaaS, custom, or on-prem)

- Internal company systems

It’s part of the broader Microsoft Entra product family, which includes services for identity governance, decentralized identity, and access management.

![image](https://github.com/user-attachments/assets/d872c0d3-4882-4ec3-8f6a-b0a71d3b55a8)

### 2. Microsoft Entra ID main feature and capabilities

#### 2.1. Single Sign-On (SSO)

Sign in once to access all applications (like Outlook, Teams, Salesforce, etc.).

Reduces password fatigue and improves user experience.

#### 2.2 Multi-Factor Authentication (MFA)

Adds an extra layer of security beyond username and password.

Examples: SMS codes, authenticator apps, biometric login.

#### 2.3 Conditional Access

Control access based on conditions like user location, device health, or risk level.

Example: Block access from risky countries, or require MFA when outside the corporate network.

#### 2.4 Identity Protection

Uses machine learning to detect and respond to suspicious login attempts.

Can automatically block or challenge high-risk sign-ins.

#### 2.5 Application Management

Centralized portal to manage app access, provisioning, and security.

Integrates with thousands of prebuilt apps (Google Workspace, ServiceNow, etc.).

#### 2.6 Device Management Integration

Works with Intune and Microsoft Endpoint Manager.

Helps enforce policies like “Only allow corporate-managed devices”.

#### 2.7 B2B and B2C Identity

B2B: Collaborate with external partners by giving them secure access to your resources.

B2C: Create branded sign-in experiences for your customers.

#### 2.8 Role-Based Access Control (RBAC)

Assign users roles that limit what they can do within applications and Azure resources.

#### 2.9 Lifecycle Management

Automate user provisioning and de-provisioning.

Sync with on-prem Active Directory if needed.

#### 2.10. Audit Logs and Monitoring

Track sign-ins, changes, and access history.

Integrate with Microsoft Sentinel for advanced SIEM (Security Info and Event Management).

### 3.Navigation Panel: Microsoft Entra ID Menu

#### 3.1. Overview and Diagnose/Solve problems

![image](https://github.com/user-attachments/assets/68679ce1-f087-4f1a-9571-58325e32aeaa)

**Overview**

Dashboard with a summary of your tenant:

- Tenant name, ID, primary domain

- Number of users, groups, apps, and devices

- Current license (e.g., Microsoft Entra ID Free)

- Alerts, announcements, and identity secure score

![image](https://github.com/user-attachments/assets/73315a69-2011-416c-9e8f-240a22c48d8c)

**Diagnose and solve problems**

Guided troubleshooting for common issues:

- Sign-in issues

- Application access problems

- Conditional Access misconfigurations

- License or provisioning issues

![image](https://github.com/user-attachments/assets/a606a6fd-4ab9-485a-a5d0-0a011304b0e0)

#### 3.2. Manage Users

![image](https://github.com/user-attachments/assets/a38c1256-94d2-4523-a70f-3476792bb050)

![image](https://github.com/user-attachments/assets/af19aee4-262d-49db-b927-a88fb0ea4cc6)

![image](https://github.com/user-attachments/assets/0475c555-48df-4de2-9d1b-ae5c82a2d301)

![image](https://github.com/user-attachments/assets/6e0d2d5f-60cf-4989-a24c-40cb51286d40)

#### 3.3. Groups

![image](https://github.com/user-attachments/assets/e3cc650d-1ef6-4bbc-b284-7ce55cdd127c)

**Overview**

A dashboard summarizing the current state of your groups:

- Total number of groups

- Types of groups: M365, security, dynamic, cloud, on-premises

- Alerts and feature suggestions (e.g., access reviews)

**All groups**

Shows all groups in your directory.

Types include:

- Security groups: Control access to apps and resources.

- Microsoft 365 groups: Used for collaboration (Teams, Outlook, SharePoint).

- Dynamic groups: Automatically add/remove members based on rules.

You can create, edit, delete, or manage memberships here.

**Deleted groups**

View and restore soft-deleted groups (kept for 30 days by default).

Useful for accidental deletion recovery.

**Diagnose and solve problems**

Run troubleshooting tools for group-related issues like:

Users not showing up in groups

Access problems with apps/resources

Sync problems (hybrid environments)

**Settings Section**

**General**

Set default group settings, including:

Group creation permissions

Who can manage groups

Visibility (public/private for M365 groups)

**Expiration**

Configure lifetime policies for groups:

Automatically expire and delete unused groups

Send renewal notifications

**Naming policy**

Define naming conventions and blocked words to control how groups are named.

Enforce prefixes/suffixes

Prevent inappropriate or confusing names

**Activity Section**

**Privileged Identity Management (PIM)**

Use just-in-time access and approval workflows for sensitive group roles.

Apply time-limited assignments for roles like Group Owner or Administrator.

**Access reviews**

Set up periodic checks to verify who should still be in a group.

Helps maintain security and compliance by removing unnecessary access.

**Audit logs**

See a history of actions related to groups:

Creation/deletion

Membership changes

Role assignments

**Bulk operation results**

Monitor the status of bulk group operations, such as:

Importing members via CSV

Bulk deletion

Group creation scripts

**Troubleshooting + Support**

New support request

Submit a ticket to Microsoft Support if you're facing group-related issues that need further help.

#### 3.4. External Identities

The External Identities section in Microsoft Entra ID allows you to securely manage external users—like partners, suppliers, customers, and guests—who access your resources

![image](https://github.com/user-attachments/assets/b9883ea8-e331-4fac-8167-adb487bb4b3a)

![image](https://github.com/user-attachments/assets/b415971c-5d84-4c31-900c-d5d16ce58da2)

![image](https://github.com/user-attachments/assets/1c4e36b7-4f2b-4806-8a49-b9e1b25a6b0e)

![image](https://github.com/user-attachments/assets/24c592aa-84b2-4d52-b4d0-f93a4fd2933f)

#### 3.5. Roles and administrators

You're in the Roles and administrators section of Microsoft Entra ID, where you manage role-based access control (RBAC) for identity and directory management.

![image](https://github.com/user-attachments/assets/211c8a15-bbe0-49ad-a3bf-34488060a849)

![image](https://github.com/user-attachments/assets/573c20ea-b367-4e03-b150-88bcc755f95e)

![image](https://github.com/user-attachments/assets/efe75bcf-777c-432a-9a8d-df1210bdee30)

![image](https://github.com/user-attachments/assets/5fae8606-8abc-4199-9c2a-148434a980ad)

#### 3.6.


#### 3.7.


#### 3.8.


#### 3.9.


### 4. Microsoft Entra Admin Center

https://entra.microsoft.com/

![image](https://github.com/user-attachments/assets/0a15d643-cb83-43fd-9617-75402055ecf3)

#### 4.1.



#### 4.2.



#### 4.3.




#### 4.4.




#### 4.5.






## AWS

### 1. What is AWS IAM?

AWS IAM stands for Identity and Access Management.

It’s a secure, centralized system in Amazon Web Services that lets you control who can access what in your AWS environment.

It’s one of the first things you set up when you create an AWS account because it defines how users and systems interact with AWS services.

With **IAM**, you can create **least-privilege policies**, which means **giving users or systems only the access they need—nothing more**.

![image](https://github.com/user-attachments/assets/312a8693-5499-47d4-b6a4-331910026e2f)

### 2. Key Concepts of AWS IAM

![image](https://github.com/user-attachments/assets/21c6cf5b-592d-46cd-bf70-935eeb6a9aae)

### 3. 

## Comparison table between AWS IAM and Microsoft Entra ID (formerly Azure AD) 

Two powerful but different **Identity (Authentication) and Access Management (Authorization)** platforms used in **AWS** and **Azure** ecosystems.

![image](https://github.com/user-attachments/assets/a4e70048-41fa-4b5d-b326-30ee729abda1)

![image](https://github.com/user-attachments/assets/55cb4984-a44b-422a-b588-9a8c3b843aa9)


## Google Cloud Services

