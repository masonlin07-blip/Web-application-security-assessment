# web-application-security-assessment
Security assessment of a web application, investigating cross-site scripting (XSS), access-control weaknesses, and database security risks.


## Overview

This project involved assessing a web application for common security vulnerabilities as part of university cybersecurity coursework.

The assessment focused on identifying cross-site scripting (XSS), investigating access-control weaknesses, and analysing database security risks. Findings were documented alongside potential impacts and recommendations for improving application security.

## Objectives

- Identify potential reflected and stored XSS vulnerabilities.
- Investigate access-control weaknesses and unauthorised data exposure.
- Analyse database-related security risks.
- Recommend mitigations to improve application security.


## Tools and Methodology

### Tools Used
- **Burp Suite** — Intercepted and modified web requests to investigate application security weaknesses.
- **Web browser and developer tools** — Used to interact with the application and examine its behaviour during testing.

### Assessment Areas
- **Cross-Site Scripting (XSS):** Investigated reflected and stored XSS vulnerabilities in user input fields.
- **Access Control:** Examined whether users could access files outside their authorised department by modifying request parameters.
- **Database Security:** Analysed potential information disclosure risks associated with database queries and exposed data.

### Approach
1. Interacted with the application to identify potential security weaknesses.
2. Tested relevant inputs and requests to investigate the identified issues.
3. Analysed the potential impact of each finding.
4. Documented findings and recommended security mitigations.

## Key Findings and Remediation

### 1. Cross-Site Scripting (XSS)
- **Finding:** Investigated reflected and stored XSS in user input fields.
- **Impact:** Potential execution of injected scripts in users' browsers.
- **Mitigation:** Apply output encoding, appropriate input validation, and Content Security Policy (CSP).

### 2. Broken Access Control
- **Finding:** Identified unauthorised file access by modifying a department identifier in a request.
- **Impact:** Exposure of files belonging to another department.
- **Mitigation:** Enforce server-side authorisation checks and least-privilege access.

### 3. Database Information Disclosure
- **Finding:** Analysed how aggregate query results could reveal sensitive information.
- **Impact:** Potential inference of confidential data.
- **Mitigation:** Restrict data access and apply appropriate privacy controls.
