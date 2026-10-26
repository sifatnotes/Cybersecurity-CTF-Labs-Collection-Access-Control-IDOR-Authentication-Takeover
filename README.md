# Cybersecurity-CTF-Labs-Collection-Access-Control-IDOR-Authentication-Takeover
A curated, searchable index of hands-on CTF labs covering IDOR, horizontal and vertical privilege escalation, OAuth account takeover, password reset poisoning, JWT algorithm confusion, and Mass Assignment from Learn SecByte.
# Access Control, IDOR & Authentication Takeover CTF Labs Collection

A structured, searchable index of hands-on cybersecurity labs focusing on Insecure Direct Object References (IDOR), Horizontal & Vertical Privilege Escalation, Mass Assignment, OAuth implementation flaws, Password Reset Poisoning, Magic Link abuse, Cookie Poisoning, and JWT Algorithm Confusion hosted on Learn SecByte.

This collection is designed for application security engineers, penetration testers, CTF competitors, security analysts, and developers learning how to audit, exploit, and remediate modern identity, authentication, and access enforcement vulnerabilities.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
  - [Insecure Direct Object References (IDOR) & Privilege Escalation](#insecure-direct-object-references-idor--privilege-escalation)
  - [Mass Assignment & Authorization Bypass](#mass-assignment--authorization-bypass)
  - [Authentication Abuses & Account Takeover (ATO)](#authentication-abuses--account-takeover-ato)
  - [Session Security, Tokens & JWT Exploitation](#session-security-tokens--jwt-exploitation)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Authentication and authorization form the defense backbone of web applications. However, subtle flaws in session handling, token validation, access checks, or identity provider integrations frequently allow attackers to access neighbor accounts, escalate privileges to administrator status, or perform full account takeovers without credentials.

This repository organizes hands-on cybersecurity labs from Learn SecByte into logical learning paths covering modern authentication mechanisms, access control models, and token security analysis.

---

## Lab Collection & Index

| Lab Title | Target Focus | Primary Category | Access Link |
| :--- | :--- | :--- | :--- |
| **Horizontal Privilege Escalation** | Access Control | User-to-User Escalation | [Access Lab](https://learn.secbyte.org/ctf/horizontal-privilege-escalation-finding-your-neighbors-secre) |
| **Vertical Privilege Escalation** | Access Control | Role-Based Escalation | [Access Lab](https://learn.secbyte.org/ctf/vertical-privilege-escalation) |
| **Privilege Escalation Foundations** | Access Control | Complete System Compromise | [Access Lab](https://learn.secbyte.org/ctf/privilege-escalation-foundations-to-final-compromise) |
| **Forced Browsing Foundations** | Reconnaissance | Unlinked Endpoint Access | [Access Lab](https://learn.secbyte.org/ctf/forced-browsing-foundations) |
| **Mass Assignment** | Application Logic | Parameter Binding Abuse | [Access Lab](https://learn.secbyte.org/ctf/mass-assignment-hidden-fields-account-abuse) |
| **IDOR Fundamentals** | Access Control | Broken Object-Level Authorization | [Access Lab](https://learn.secbyte.org/ctf/idor-fundamentals-broken-access-control) |
| **Password Reset Poisoning** | Authentication | Host Header / Trust Abuse | [Access Lab](https://learn.secbyte.org/ctf/password-reset-poisoning-from-trust-abuse-to-defense) |
| **Magic Link Abuse** | Authentication | Passwordless Account Takeover | [Access Lab](https://learn.secbyte.org/ctf/magic-link-abuse-passwordless-account-takeover) |
| **OAuth Account Takeover** | Authentication | IdP Integration Flaws | [Access Lab](https://learn.secbyte.org/ctf/oauth-account-takeover) |
| **Cookie Poisoning & Session Fixation** | Session Security | Session Management Abuse | [Access Lab](https://learn.secbyte.org/ctf/cookie-poisoning-session-fixation-signed-cookie-abuse) |
| **Refresh Token Abuse** | Token Security | OAuth / OIDC Token Revocation | [Access Lab](https://learn.secbyte.org/ctf/refresh-token-abuse) |
| **JWT Algorithm Confusion** | Token Security | Key Confusion & Signature Bypass | [Access Lab](https://learn.secbyte.org/ctf/jwt-algorithm-confusion) |

---

## Categories

### Insecure Direct Object References (IDOR) & Privilege Escalation
Hands-on CTF labs detailing object-level authorization failures, forced endpoint discovery, and privilege boundary crossings:

* **IDOR Fundamentals:** Identifying and exploiting unvalidated direct object references in user identifiers, keys, and session parameters.
  * Lab Link: https://learn.secbyte.org/ctf/idor-fundamentals-broken-access-control
* **Horizontal Privilege Escalation:** Accessing unauthorized resources belonging to adjacent peer users.
  * Lab Link: https://learn.secbyte.org/ctf/horizontal-privilege-escalation-finding-your-neighbors-secre
* **Vertical Privilege Escalation:** Bypassing permission matrices to escalate privileges from standard user to administrator.
  * Lab Link: https://learn.secbyte.org/ctf/vertical-privilege-escalation
* **Privilege Escalation Foundations:** Methodologies for escalating access from initial low-privilege entry to final system compromise.
  * Lab Link: https://learn.secbyte.org/ctf/privilege-escalation-foundations-to-final-compromise
* **Forced Browsing Foundations:** Discovering hidden, unlinked administrative endpoints and restricted application resources.
  * Lab Link: https://learn.secbyte.org/ctf/forced-browsing-foundations

### Mass Assignment & Authorization Bypass
Practical security labs demonstrating how framework auto-binding can lead to account modification and administrative takeover:

* **Mass Assignment:** Injecting hidden fields and unexpected properties into API payloads to overwrite sensitive object attributes (`is_admin`, `role`).
  * Lab Link: https://learn.secbyte.org/ctf/mass-assignment-hidden-fields-account-abuse

### Authentication Abuses & Account Takeover (ATO)
Labs focused on subverting password recovery flows, passwordless authentication systems, and federated identity protocols:

* **Password Reset Poisoning:** Abusing HTTP Host headers and trusted proxy headers to redirect password reset tokens to attacker-controlled servers.
  * Lab Link: https://learn.secbyte.org/ctf/password-reset-poisoning-from-trust-abuse-to-defense
* **Magic Link Abuse:** Exploiting weaknesses in passwordless authentication links, email token lifetime, and predictable tokens.
  * Lab Link: https://learn.secbyte.org/ctf/magic-link-abuse-passwordless-account-takeover
* **OAuth Account Takeover:** Subverting OAuth 2.0 / OpenID Connect flows through redirect URI manipulation, missing state parameters, and token hijacking.
  * Lab Link: https://learn.secbyte.org/ctf/oauth-account-takeover

### Session Security, Tokens & JWT Exploitation
Security labs covering cryptographic token manipulation, signature verification bypasses, and session state hijacking:

* **Cookie Poisoning & Session Fixation:** Manipulating signed cookies and fixing session IDs to hijack authenticated user sessions.
  * Lab Link: https://learn.secbyte.org/ctf/cookie-poisoning-session-fixation-signed-cookie-abuse
* **Refresh Token Abuse:** Exploiting missing refresh token rotation, improper expiration policies, and token reuse vulnerabilities.
  * Lab Link: https://learn.secbyte.org/ctf/refresh-token-abuse
* **JWT Algorithm Confusion:** Forging valid JSON Web Tokens by forcing HMAC public key signing (RS256 to HS256 key confusion attacks).
  * Lab Link: https://learn.secbyte.org/ctf/jwt-algorithm-confusion

---

## Learning Path

Follow this structured roadmap to master access control auditing and authentication security:

1. **Object-Level & Role-Based Access Controls**
   - Test applications for IDOR vulnerabilities and forced browsing endpoints.
   - Practice horizontal and vertical privilege escalation vectors.
2. **Framework Binding & Mass Assignment**
   - Audit API endpoints for auto-binding vulnerabilities and parameter injection.
3. **Authentication Flows & Account Takeover**
   - Evaluate password reset mechanisms for Host header injection and token disclosure.
   - Test passwordless magic links and audit OAuth 2.0 grant types and state validation.
4. **Session Management & Token Cryptography**
   - Intercept and tamper with session cookies and test for session fixation.
   - Perform JWT signature bypasses using algorithm confusion and key misuse techniques.

---

## How to Use the Labs

1. Select a practice scenario from the index table or category breakdown above.
2. Launch the interactive target lab environment directly on Learn SecByte.
3. Use web proxies (e.g., Burp Suite) to inspect JSON bodies, alter token signatures, modify HTTP headers, and capture authentication parameters.
4. Review defensive guidelines to learn how server-side access control checks, explicit property binding, proper token validation, and strict OAuth configurations protect applications.

---

## Disclaimer

This repository is strictly intended for educational research, authorized security testing, and defensive engineering training. All concepts, techniques, and lab environments are provided to help cybersecurity practitioners identify vulnerabilities and harden modern identity systems. Unsanctioned testing or attacks against external infrastructure without prior written authorization are strictly illegal.
