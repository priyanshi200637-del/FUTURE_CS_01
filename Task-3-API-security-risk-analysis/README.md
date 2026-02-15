# Task 3 – API Security Risk Analysis

## Introduction
API security focuses on protecting application programming interfaces from attacks and misuse. 
APIs are widely used in modern applications, making them a common target for attackers.

This task analyzes common API security risks based on the OWASP API Security Top 10 and suggests 
mitigation techniques to reduce vulnerabilities.

## Scope of Analysis
- Authentication & Authorization
- Data Exposure
- Rate Limiting
- Input Validation
- Logging & Monitoring

## Tools & References
- OWASP API Security Top 10
- Postman (for API testing)
- Browser Developer Tools
- Security Best Practices Documentation

## Common API Security Risks

### 1. Broken Object Level Authorization (BOLA)
APIs fail to properly check whether a user has access to specific objects.

*Impact:* Unauthorized data access  
*Mitigation:* Enforce object-level access checks on every request.

### 2. Broken Authentication
Weak or missing authentication mechanisms.

*Impact:* Account takeover  
*Mitigation:* Use strong authentication, OAuth 2.0, JWT with expiration.

### 3. Excessive Data Exposure
APIs return more data than necessary.

*Impact:* Sensitive information leakage  
*Mitigation:* Return only required fields and use response filtering.

### 4. Lack of Rate Limiting
Unlimited API requests allowed.

*Impact:* Brute force & DoS attacks  
*Mitigation:* Implement request rate limits and throttling.

### 5. Injection Attacks
APIs accept unvalidated input.

*Impact:* Data manipulation or system compromise  
*Mitigation:* Validate and sanitize all user inputs.

## Risk Severity Table

| Risk | Severity | Impact |
|-----|--------|--------|
| BOLA | High | Data breach |
| Broken Authentication | High | Account compromise |
| Excessive Data Exposure | Medium | Privacy issues |
| No Rate Limiting | Medium | Service disruption |
| Injection | High | System damage |

## Conclusion
API security is critical for protecting modern applications. By following OWASP API Security 
best practices and implementing proper controls, organizations can significantly reduce risks 
and improve overall security posture.
