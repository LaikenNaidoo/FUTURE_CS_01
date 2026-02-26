# FUTURE_CS_01

## Passive Web Application Vulnerability Assessment

---

## Overview

This repository contains a structured Passive Web Application Vulnerability Assessment conducted as part of the Future Interns Cyber Security track.

The objective of this assessment was to identify observable security weaknesses using ethical, read-only testing techniques and present findings in a professional, business-oriented format.

The assessment focused on:

- Identifying common web security misconfigurations  
- Classifying risk severity (High / Medium / Low / Informational)  
- Explaining security impact in business-friendly language  
- Providing practical remediation recommendations  

All testing was conducted using strictly non-intrusive and passive techniques.

---

## Target Application

**Public Demo Application:**  
http://testphp.vulnweb.com  

Scope was limited to publicly accessible pages and client-side components.

The assessment did **not** include:

- Authentication bypass attempts  
- Exploitation of vulnerabilities  
- Brute-force testing  
- Denial-of-Service (DoS) activity  
- Internal infrastructure analysis  

---

## Methodology

Testing was conducted using:

- OWASP ZAP (Passive Mode)  
- Firefox Browser (proxied through ZAP)  

Manual browsing was performed to allow passive inspection of:

- HTTP response headers  
- Cookie security attributes  
- Client-side protections  
- Information disclosure via server responses  

No active scanning modules or exploitation tools were used during this engagement.

---

## Risk Summary

| Risk Level     | Count |
|---------------|--------|
| High Risk     | 0      |
| Medium Risk   | 3      |
| Low Risk      | 5      |
| Informational | 4      |

**Overall Security Posture: Moderate Risk**

---

## Medium Risk Findings (Priority)

- Content Security Policy (CSP) Header Not Set  
- Absence of Anti-CSRF Tokens  
- Missing Anti-Clickjacking Header  

These findings may increase exposure to:

- Cross-Site Scripting (XSS)  
- Clickjacking  
- Unauthorized request execution  

Immediate remediation of Medium-risk findings is recommended.

---

## Deliverables

- Vulnerability Assessment Report (PDF)  
- Supporting Evidence (OWASP ZAP screenshots)
