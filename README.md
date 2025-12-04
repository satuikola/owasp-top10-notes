<h1 align="center">🛡️ OWASP Top 10 notes and comparison (2017 vs 2021)</h1>

<p align="center">
Structured notes about the OWASP Top 10 with practical explanations, a 2017 to 2021 comparison and real world examples.
</p>

---

> This repository is based on a course assignment where I analyzed both the 2017 and 2021 OWASP Top 10 lists and compared how the risk landscape has changed.

---

## Quick navigation

<!-- toc -->
<!-- tocstop -->

---

## 1. Goal of this repository

The aim of this repo is to provide:

- an overview of the OWASP Top 10 (2021)
- a concise comparison between 2017 and 2021
- real world scenarios for the main categories
- a portfolio friendly example of how I communicate security concepts

---

## 2. OWASP Top 10 2021 overview

### A01 - Broken Access Control

Access control failures allow users to perform actions outside their permissions.

### A02 - Cryptographic Failures

Insufficient protection of data in transit or at rest.

### A03 - Injection

Untrusted input becomes part of a command or query.  
Includes for example SQL injection, NoSQL injection, LDAP injection, command injection and XSS.

### A04 - Insecure Design

Lack of security consideration during early design phases, missing threat modelling and unsafe workflows.

### A05 - Security Misconfiguration

Incorrect or unsafe settings, unnecessary features and default credentials.  
Also includes parts of the former XML External Entities (XXE) category.

### A06 - Vulnerable and Outdated Components

Using libraries or dependencies with known vulnerabilities.

### A07 - Identification and Authentication Failures

Weak authentication, missing MFA and poor session handling.

### A08 - Software and Data Integrity Failures

Unverified updates, compromised CI or CD pipelines and tampering risks.

### A09 - Security Logging and Monitoring Failures

Renamed and updated from 2017. Missing logs or alerts allow attacks to go unnoticed.

### A10 - Server-Side Request Forgery (SSRF)

User controlled input can trigger unintended server requests.

---

## OWASP Top 10 – Comparison: 2017 → 2021

| **2017 Category** | **2021 Status** |
|-------------------|-----------------|
| **Injection** | Still present, now more broadly defined. <br>Includes **SQL**, **NoSQL**, **LDAP**, **command injection**, and **XSS**. |
| **Broken Authentication** | Merged into **Identification and Authentication Failures**, covering weak login mechanisms and session handling. |
| **Sensitive Data Exposure** | Renamed as **Cryptographic Failures**, with stronger emphasis on protecting data in transit and at rest. |
| **XML External Entities (XXE)** | Merged into both **Injection** and **Security Misconfiguration**, reflecting its dual nature. |
| **Broken Access Control** | Elevated to **A01** in 2021, highlighting its increased prevalence and impact in real-world breaches. |
| **Security Misconfiguration** | Still present, now expanded to include broader misconfigurations and parts of **XXE**. |
| **Cross-Site Scripting (XSS)** | Absorbed into **Injection**, no longer listed as a standalone category. |
| **Insecure Deserialization** | Reclassified under **Software and Data Integrity Failures**, focusing on trust boundaries and update mechanisms. |
| **Using Components with Known Vulnerabilities** | Still present as **Vulnerable and Outdated Components**, emphasizing dependency management. |
| **Insufficient Logging and Monitoring** | Renamed to **Security Logging and Monitoring Failures**, with broader scope including alerting and visibility gaps. |

📎 For detailed analysis and examples, see:  
🔗[Detailed comparison](docs/OWASP_2017_vs_2021_detailed.md)


---

## 4. Real world scenarios

Examples of how these categories can appear in practice:

- **Broken Access Control**: URL manipulation reveals another user’s data  
- **Security Logging Failure**: brute force attempts generate no alerts  
- **Insecure Design**: a feature is built without rate limiting, so endless login attempts are possible  
- **Vulnerable Components**: a known vulnerable library is never updated

📎 More scenarios are listed in:  
🔗 [Real-world scenarios](docs/Real_world_scenarios.md)



---

## 5. What I learned

From this analysis I concluded that:

- OWASP 2021 focuses more on design level flaws, access control problems and integrity failures
- supply chain and CI/CD (continuous integration / continuous delivery)–related risks are now clearly visible in the Top 10.
- several older categories were consolidated to better reflect modern attack patterns

These observations match real world incidents where broken access control and weak logging often play a central role.

---

## 6. Notes about the original assignment

The original assignment was written as part of my cybersecurity studies and included:

- a comparison of OWASP Top 10 2017 and 2021
- written reflections on why some categories moved or were renamed
- examples linked to typical web applications

This repository is a cleaned up and English language version of that work.  

📎 Short notes from the original assignment are in:  
🔗 [Notes from assignment](docs/Notes_from_assignment.md)


---

## 7. About this repository

This repository is part of my cybersecurity learning journey and portfolio.  
It demonstrates my understanding of web application risks and my ability to:

- map my notes to industry standard frameworks like OWASP
- communicate technical security topics in clear language
