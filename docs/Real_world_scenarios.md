# Real world scenarios for OWASP Top 10

Below are simplified examples that demonstrate how each OWASP category may appear in real systems.  
These examples help illustrate how the vulnerabilities manifest in practical situations and why they matter.

---

## A01 — Broken Access Control

A user changes `?id=100` to `?id=101` in a URL and gains access to another user’s profile or sensitive information.  
This happens when authorization checks are missing or inadequate.

---

## A02 — Cryptographic Failures

A login page uses HTTP instead of HTTPS, causing credentials to be transmitted in cleartext.  
Attackers can capture the traffic with a simple network sniffer.

Another example: passwords stored without hashing or with outdated algorithms like MD5.

---

## A03 — Injection

User input is inserted directly into a database query:

```sql
SELECT * FROM users WHERE username = '$input';
