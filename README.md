# AWS IAM Identity Center — Multi-Account Access Lab

## Overview

This lab demonstrates centralized workforce access management using **AWS IAM Identity Center** across an AWS Organization.

Users and groups were created in IAM Identity Center and assigned permission sets to provide controlled access to multiple AWS accounts.

---

## Architecture

```text
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
