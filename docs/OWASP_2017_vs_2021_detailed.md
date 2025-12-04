# OWASP Top 10 detailed comparison (2017 vs 2021)

This document provides a deeper comparison of the OWASP Top 10 lists from 2017 and 2021, including changes in structure, terminology and risk prioritization.

---

## Key differences at a glance

Some major observations:

- Broken Access Control moved from A05 to A01 because of real world breach trends
- Insecure Design was added to emphasize shift left and secure architecture
- Software and Data Integrity Failures reflects the rise of supply chain attacks
- Cryptographic Failures replaces Sensitive Data Exposure with clearer terminology
- XXE and XSS are no longer standalone categories

---

## Category by category breakdown

### 2017 A1 Injection → 2021 A03 Injection

Still present but broadened. Includes SQL injection, NoSQL injection, LDAP injection, command injection, XSS and some XXE patterns.

### 2017 A2 Broken Authentication → 2021 A07 Identification and Authentication Failures

Expanded to cover multi factor authentication issues, credential stuffing, session fixation and similar problems.

### 2017 A3 Sensitive Data Exposure → 2021 A02 Cryptographic Failures

Clarifies focus on missing, weak or broken cryptographic controls rather than only “data exposure” symptoms.

### 2017 A4 XML External Entities (XXE) → 2021 merged into A03 Injection and A05 Security Misconfiguration

XXE test cases now appear under both categories depending on the nature of the vulnerability.  
For example:

- unsafe XML parser configuration can map to Security Misconfiguration  
- XXE payloads that lead to data exfiltration through injected entities can map to Injection

### 2017 A5 Broken Access Control → 2021 A01 Broken Access Control

Now the highest ranking risk. Widely seen in real breaches, for example insecure object references and missing authorization checks.

### 2017 A6 Security Misconfiguration → 2021 A05 Security Misconfiguration

Broader than before. Includes cloud misconfigurations, unnecessary services, default accounts and several settings that used to be spread across multiple categories, including parts of XXE.

### 2017 A7 Cross Site Scripting (XS
