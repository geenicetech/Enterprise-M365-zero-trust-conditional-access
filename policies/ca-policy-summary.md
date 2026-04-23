# Conditional Access Policy Summary

---

## Purpose

This document summarizes the Conditional Access policies implemented in the Microsoft 365 tenant to support a Zero Trust identity security model.

---

## Policy Overview

### Policy 1: Require MFA for All Users
**Objective:**  
Protect all user and administrator accounts from credential-based attacks.

**Scope:**  
- Users: All users  
- Cloud apps: All cloud apps  

**Controls:**  
- Grant access only after MFA  
- Break-glass account excluded  

---

### Policy 3: Block Legacy Authentication
**Objective:**  
Prevent authentication methods that bypass modern security controls.

**Scope:**  
- Users: All users  
- Client apps: Legacy authentication protocols  

**Controls:**  
- Block access  
- Break-glass account excluded  

---

## Break-Glass Account Handling

- Excluded from all Conditional Access policies
- Used only in emergency loss-of-access scenarios
- Not used for routine administration

---

## Governance Principles Applied

- Zero Trust: Never trust, always verify
- Least privilege
- Defense against credential attacks
- Administrative access risk reduction

---

## Review & Maintenance

- Policies should be reviewed periodically
- Sign-in logs should be monitored for unexpected behavior
- Break-glass access should be tested safely and infrequently
