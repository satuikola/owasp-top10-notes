# Notes from my original OWASP assignment

These notes summarize the key insights from the original course assignment where I analyzed the OWASP Top 10 (2017 vs 2021) from a learning and practical perspective.

The purpose of the assignment was to compare how the focus areas of web application security have changed over time, and to reflect on why certain risks became more prominent.

---

## Key observations from the assignment

### 1. Major shifts between 2017 and 2021
- **Broken Access Control** became the number one risk in 2021 (A01), reflecting its prominence in real-world breaches.
- **Insecure Design** was added as a new category, highlighting the industry's move toward “shift-left” security.
- **Software and Data Integrity Failures** appeared due to the rise of supply chain attacks and CI/CD pipeline risks.
- **Sensitive Data Exposure** was redefined more precisely as **Cryptographic Failures**.

---

## 2. Consolidation of categories

Several 2017 categories were reorganized:

- **XSS** was absorbed under **Injection** rather than existing as its own entry.  
- **XXE** was split between **Injection** and **Security Misconfiguration** depending on context.  
- **Insecure Deserialization** migrated into **Software and Data Integrity Failures**.

This consolidation made the list more aligned with real-world attack patterns.

---

## 3. Increased emphasis on secure design and architecture

The 2021 list shows a clear industry shift:

- Security must be built in early, not bolted on later.
- Missing security requirements in the design stage lead to systemic vulnerabilities.
- Threat modeling and architectural review are now essential practices.

---

## 4. Real-world breach relevance

The assignment highlighted several examples where:

- lack of access control  
- failure to patch dependencies  
- weak authentication  
- and missing logging  

directly contributed to major incidents.

Many well-known breaches map cleanly to OWASP categories, which reinforces why the updated Top 10 matters.

---

## 5. Personal takeaway

From completing the assignment, I learned:

- how OWASP Top 10 evolves over time  
- why certain vulnerabilities rise or fall in priority  
- how to connect theoretical categories to real-world attack scenarios  
- how to read OWASP material with a critical and analytical mindset  

This repo is a cleaned-up, portfolio-friendly version of those insights.

---

## Additional context

These notes were originally written as part of cybersecurity studies focusing on:

- web application security fundamentals  
- secure coding and architecture  
- threat modeling
