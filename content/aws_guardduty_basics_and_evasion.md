---
author_name: Karthick
title: AWS GuardDuty Basics and Detection Overview
description: Explains AWS GuardDuty, what it detects, and basic attacker evasion concepts
---

## What is AWS GuardDuty?

Amazon GuardDuty is a threat detection service that continuously monitors AWS accounts and workloads for malicious activity.

It uses logs from:
- CloudTrail
- VPC Flow Logs
- DNS logs

to detect suspicious behavior.

---

## What does GuardDuty detect?

GuardDuty can detect:
- Unauthorized access attempts
- Unusual API calls
- Crypto mining activity
- Suspicious network traffic
- Known malicious IP interactions

---

## Why is it important?

It helps organizations:
- Detect attacks early
- Monitor AWS account misuse
- Identify compromised credentials
- Improve cloud security visibility

---

## How attackers think about GuardDuty

Attackers don’t “disable” GuardDuty directly, but they try to:
- Avoid noisy actions that trigger alerts
- Use stealthier API calls
- Blend with normal user behavior
- Reduce detectable patterns

---

## Example scenario

An attacker gains AWS credentials and tries to access resources.

If they perform unusual actions (like listing all S3 buckets rapidly), GuardDuty may flag suspicious behavior.

---

## How to reduce risks (defender side)

- Enable GuardDuty in all regions
- Monitor alerts regularly
- Integrate with SIEM tools
- Use least privilege IAM policies
