# AWS Cloud Security Monitoring & SOC Log Analysis

## 📌 Project Overview
This project demonstrates basic cloud security monitoring using AWS native services. The main goal was to understand how a Security Operations Center (SOC) analyst monitors and investigates cloud-based activities such as user logins and system events.

The lab was implemented using AWS Free Tier services and focuses on defensive security practices.

---

## 🎯 Objectives
- Secure AWS root account using MFA
- Implement least-privilege IAM access
- Deploy and harden an EC2 instance
- Enable AWS CloudTrail for logging
- Analyze authentication and activity logs

---

## 🛠️ Technologies Used
- AWS IAM
- AWS EC2
- AWS CloudTrail
- Amazon S3

---

## 🔐 Security Implementation
- Enabled Multi-Factor Authentication (MFA) for root account
- Created a restricted IAM user (soc-analyst)
- Applied least-privilege access policies (SecurityAudit, ViewOnlyAccess)
- Configured SSH access with key-based authentication
- Restricted network access using security groups

---

## 📊 Log Monitoring & Analysis
CloudTrail was used to monitor and analyze AWS activities.

Key events analyzed:
- ConsoleLogin (user authentication)
- SendSSHPublicKey (SSH access)

Attributes reviewed:
- Timestamp
- User identity
- Source IP address
- MFA status

---

## 🔍 Investigation Summary
A ConsoleLogin event was analyzed:
- Login was successful
- Source IP matched expected location
- MFA was enabled
- No suspicious activity detected

All events were classified as legitimate after analysis.

---

## 🧠 Key Learnings
- Understanding of AWS security best practices
- Hands-on experience with CloudTrail logging
- Practical exposure to SOC investigation workflows
- Ability to analyze and validate authentication events

---

## 📄 Project Report
Full report is included in this repository.

---

## 🚀 Author
Kaveen Chandupa
