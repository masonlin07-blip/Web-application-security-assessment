
# Web Application Security Assessment

Security assessment of a web application as part of university cybersecurity coursework.

(Disclaimer both projects were simulated environments, any private information is fiction)

## Objectives
- Identify reflected and stored cross-site scripting (XSS).
- Investigate access-control weaknesses and data exposure.
- Analyse database security risks and recommend mitigations.

## Tools
- **Burp Suite** — Intercepting and modifying HTTP requests.
- **Browser tools** — Testing application behaviour.

## Key Findings

### Cross-Site Scripting (XSS)
- Investigated reflected and stored XSS in user input fields.
- **Mitigation:** Output encoding and appropriate input validation.

### Broken Access Control
- Identified unauthorised access to another department's files by modifying a request parameter.
- **Mitigation:** Server-side authorisation checks and least-privilege access.

### Database Information Disclosure
- Analysed how aggregate query results could reveal sensitive information.
- **Mitigation:** Restrict data access and apply privacy controls.

## Key Takeaways
Gained practical experience in web application security testing, vulnerability analysis, and documenting remediation recommendations.


