# Enterprise Zero Trust Identity Access
## Microsoft 365 Conditional Access Implementation

---

## Project Overview

This project demonstrates the implementation of **Zero Trust identity access controls** in a Microsoft 365 tenant using **Conditional Access policies**.

The goal is to protect user and administrator identities by enforcing strong authentication requirements, reducing credential-based attacks, and aligning access decisions with modern security best practices.

---

## Business Problem

Passwords alone are no longer sufficient to protect cloud identities.  
Common risks include:

- Password spraying and brute-force attempts
- Administrative account compromise
- Legacy authentication protocols bypassing MFA
- Inconsistent access controls across users and roles

Without Conditional Access, Microsoft 365 tenants remain vulnerable even when MFA is enabled.

---

## Solution Implemented

A baseline **Zero Trust Conditional Access model** was implemented using Microsoft Entra Conditional Access, focusing on:

- Universal MFA enforcement
- Blocking legacy authentication protocols
- Preserving emergency access via a break-glass account

---

## Zero Trust Conditional Access Flow

The access decision process follows a Zero Trust model:

1. User attempts sign-in
2. Identity is evaluated
3. Conditional Access policies are applied
4. Grant or block decision is enforced

See diagram:
diagrams/conditional-access-zero-trust-flow.png

---

## Conditional Access Policies Implemented

### 1. Require MFA for All Users
- Applies to all users
- Requires MFA for access to all cloud apps
- Break-glass account explicitly excluded

### 3. Block Legacy Authentication
- Blocks legacy authentication clients
- Prevents MFA bypass
- Break-glass account explicitly excluded

---

## Validation & Testing

Policies were validated using:
- Test user accounts
- Microsoft Entra sign-in logs
- Policy application results

Successful enforcement was confirmed through sign-in log evaluation.

See diagram:
diagrams/CA-sign-in-logs-validation.png

---

## Security Benefits Achieved

- Significant reduction in identity attack surface
- MFA enforced consistently across the tenant
- Administrative access hardened
- Legacy authentication risks eliminated
- Emergency access preserved without weakening security posture

---

## Tools & Technologies

- Microsoft Entra Admin Center
- Microsoft Entra Conditional Access
- Microsoft 365 identity platform
- Microsoft Entra sign-in logs

---

## Status

✅ Completed  
This project establishes a secure foundation for identity protection and supports future compliance and security initiatives.
