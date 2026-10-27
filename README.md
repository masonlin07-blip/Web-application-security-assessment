
# Web Application Security Assessment

Security assessment of a web application as part of university cybersecurity coursework
(Disclaimer project was a simulated environment, all private information is fictional)

## Objectives
- Test for reflected and stored cross-site scripting (XSS)
- Investigate broken access control and unauthorised data exposure
- Document vulnerabilities and recommend security mitigations

## Tools
- **Burp Suite** — Intercepting and modifying HTTP requests
- **Browser developer tools** — Inspecting application behaviour

## Key Findings

### 1. Cross-Site Scripting (XSS)
- Tested reflected XSS in the login and chat search features, and stored XSS in chat messages
- Observed JavaScript execution through browser alert pop-ups
- **Mitigation:** Apply context-aware output encoding and appropriate input validation

### 2. Broken Access Control
- Modified a request parameter to access files belonging to another department
- Demonstrated that the application did not adequately enforce server-side authorisation
- **Mitigation:** Enforce server-side access checks on every request and apply least-privilege principles

## Evidence
Screenshots are provided in the `screenshots/` directory to demonstrate selected test results

## Detailed Findings

See [FINDINGS.md](FINDINGS.md) for testing methods, observed results, potential impacts, and recommended mitigations

## Key Takeaways
Developed practical experience in web application security testing, vulnerability analysis, HTTP request inspection, and remediation recommendations


