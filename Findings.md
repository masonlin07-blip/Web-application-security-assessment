# Security Assessment Findings

## Overview
University cybersecurity coursework assessing web application security using browser testing and Burp Suite

## 1. Cross-Site Scripting (XSS)

**Vulnerabilities tested:**
- **Reflected XSS:** Login username input
- **Stored XSS:** Company chat messages
- **Reflected XSS:** Company chat search

**Findings:** Test inputs triggered JavaScript execution in all three tested areas, demonstrating improper handling of user-supplied input

**Mitigations:** Apply context-aware output encoding, safely handle user-generated content, and avoid inserting untrusted input directly into HTML

## 2. Broken Access Control

**Finding:** Modified the `department_id` parameter in a file download request using Burp Suite. An Engineering test account received HR department file content without the expected authorisation checks

**Potential Impact:** Unauthorised access to confidential departmental information

**Mitigations:** Enforce server-side authorisation for every resource request, verify user permissions, and apply least-privilege access controls

## Tools
- **Burp Suite** — HTTP request interception and modification
- **Web browser** — Testing application behaviour and observing results

## Key Takeaway
Gained practical experience in web vulnerability testing, analysing HTTP requests and responses, assessing security risks, and recommending remediation


