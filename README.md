# FUTURE_CS_01
# # 🔐 Passive Web Application Vulnerability Assessment  

# 📌 Overview  

This repository contains a professional **Passive Web Application Vulnerability Assessment** conducted using **OWASP ZAP (Passive Mode)**.

The objective of this assessment was to:

- Identify common web security weaknesses  
- Classify risks based on severity (High / Medium / Low / Informational)  
- Explain technical findings in clear, business-friendly language  
- Provide practical and actionable remediation recommendations  

All testing was conducted using strictly **read-only, non-intrusive techniques**.

---

## 🌐 Target Application  

Public Demo Application:  
http://testphp.vulnweb.com  

Scope was limited to publicly accessible pages only.  

The assessment did **not** include:

- Authentication bypass attempts  
- Exploitation of vulnerabilities  
- Brute-force testing  
- Denial-of-Service (DoS) activity  
- Internal infrastructure testing  

---

## 🛠 Methodology  

The assessment was conducted using:

- **OWASP ZAP (Passive Mode)**  
- **Firefox Browser (Proxied Through ZAP)**  

Manual browsing was performed to allow passive inspection of:

- HTTP response headers  
- Cookie configurations  
- Client-side security controls  
- Information disclosure through server responses  

No active scanning modules were enabled.

---

## 📊 Risk Summary  

| Risk Level     | Count |
|---------------|--------|
| High Risk     | 0      |
| Medium Risk   | 3      |
| Low Risk      | 5      |
| Informational | 4      |

---

## 🚨 Medium Risk Findings  

- Content Security Policy (CSP) Header Not Set  
- Absence of Anti-CSRF Tokens  
- Missing Anti-Clickjacking Header  

These findings should be prioritised to reduce exposure to client-side attacks such as Cross-Site Scripting (XSS), clickjacking, and unauthorized request execution.

---

## 📁 Repository Structure  
