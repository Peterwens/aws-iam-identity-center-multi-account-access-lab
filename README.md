# AWS IAM Identity Center — Multi-Account Access Lab

## Overview

This lab demonstrates centralized workforce access management using **AWS IAM Identity Center** across an AWS Organization.

Users and groups were created in IAM Identity Center and assigned permission sets to provide controlled access to multiple AWS accounts.

---

## Architecture

What Was Implemented
IAM Identity Center organization instance
Workforce users
Security and administrator groups
AdministratorAccess permission set
Multi-account access
Permission-set provisioning
Organization integration
Delegated administration configuration
Access Model
User
  │
  ▼
Group
  │
  ▼
Permission Set
  │
  ▼
AWS Account
  │
  ▼
AWS Access
Validation
Users and Groups

Users and groups were successfully created in IAM Identity Center.

Result: PASS ✅

Permission Set

The AdministratorAccess permission set was successfully created and provisioned.

Result: PASS ✅

Multi-Account Access

AWS accounts from the organization were successfully made available through IAM Identity Center.

Result: PASS ✅

Security Concepts
Centralized Identity

IAM Identity Center provides centralized workforce identity and access management across multiple AWS accounts.

Groups

Groups allow permissions to be managed for multiple users instead of assigning access individually.

Permission Sets

Permission sets define the permissions users receive when accessing AWS accounts.

Multi-Account Access

Users can access multiple AWS accounts through a centralized identity system.

Key Result

The lab successfully demonstrated centralized workforce identity and multi-account AWS access using AWS IAM Identity Center.

Technologies
AWS IAM Identity Center
AWS Organizations
IAM Groups
Permission Sets
AWS Accounts
AWS Management Console
Disclaimer

This repository represents a personal AWS security laboratory environment.

No passwords, credentials, access keys, or secrets are included.

Sensitive account information has been redacted from public screenshots.



                    AWS Organization
                           │
                           ▼
                AWS IAM Identity Center
                           │
              ┌────────────┼────────────┐
              │            │            │
            Users        Groups    Permission Sets
              │            │            │
              └────────────┼────────────┘
                           ▼
                     AWS Accounts
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
       Infrastructure   Sandbox       Security
                           │
                        Workload
