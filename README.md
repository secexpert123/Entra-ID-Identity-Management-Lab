# Microsoft Entra ID: Identity Management & Security Lab

This project demonstrates how to design and manage cloud-based identity and access controls using Microsoft Entra ID...

## Table of Contents
1. [Project Overview](#project-overview)
2. [Lab Overview](#lab-overview)
3. [Identity Management Walkthrough](#identity-management-walkthrough)
4. [Security Hardening](#phase-2-security-hardening-mfa--sspr)
5. [RBAC & Group Management](#phase-3-rbac--scalable-group-infrastructure)
6. [Verification & Auditing](#phase-4-verification--sign-in-auditing)
7. [Technical Skills Used](#technical-skills-used)

## Lab Overview
This lab focuses on:
Cloud-only user lifecycle management
MFA and Self-Service Password Reset (SSPR) configuration
Role-Based Access Control (RBAC)
Group creation and membership validation
Reviewing sign‑in logs and identity attributes
Each step is documented with screenshots to show the full IAM workflow.

## Identity Management Walkthrough
Below is the complete step-by-step documentation of your work, with each screenshot explained clearly.

1. User Creation: 
Created a cloud-only user for the Technical Support role. Verified UPN, Object ID, and directory attributes to ensure proper identity provisioning.

![User Creation](01-User-Creation.png)
![User Overview](03-User-Technical-Details.png)

## Phase 2: Security Hardening (MFA & SSPR)
**Objective:** Secure the tenant and reduce administrative overhead for password resets.
* Enforced Multi-Factor Authentication (MFA) and Self-Service Password Reset (SSPR).
* Registered a recovery email and phone number to provide account redundancy and resilience.

![MFA Configuration](04-MFA-Phone-Email-Setup.png)
![Recovery Email](05-Recovery-Email-Config.png)

## Phase 3: RBAC & Scalable Group Infrastructure
**Objective:** Apply the "Principle of Least Privilege" and organize users into functional units.
* Assigned the **Teams Communications Support Engineer** role to limit access to necessary functions only.
* Built a Security Group named `IT-Support-Team` to demonstrate scalable permission management.

![RBAC Role Assignment](06-RBAC-Teams-Role.png)
![Group Creation](07-Group-Creation.png)
![Group Membership](08-Group-Membership-Confirm.png)

## Phase 4: Verification & Sign-in Auditing
**Objective:** Verify that security policies and permissions are functioning correctly.
* Analyzed the **Sign-in Logs** to confirm a successful authentication event.
* Verified the "Lyckades" (Success) status, confirming that the MFA challenge was passed and access was granted.

![Sign-in Logs](09-Final-Success-Log.png)

## Technical Skills Used
* **Directory Administration:** Identity lifecycle management in Entra ID.
* **Identity Security:** Configuration of MFA, SSPR, and authentication methods.
* **Access Control:** Role-Based Access Control (RBAC) and Security Group architecture.
* **Governance & Auditing:** Interpreting Sign-in and Audit logs for compliance.
