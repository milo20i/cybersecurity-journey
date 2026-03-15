# IDOR — TryHackMe

## Overview

This lab focuses on **IDOR (Insecure Direct Object References)**, a common web vulnerability related to **broken access control**.

IDOR occurs when an application exposes internal object references (such as user IDs or file identifiers) without properly verifying whether the user is authorized to access them.

Attackers can exploit this by manipulating identifiers to access resources belonging to other users.

---

## What is an IDOR?

An IDOR vulnerability happens when a web application allows direct access to objects based on user-controlled input.

For example:

```
https://example.com/profile?user_id=123
```

If the application does not verify whether the logged-in user owns that resource, an attacker could modify the ID:

```
https://example.com/profile?user_id=124
```

This may expose **another user's data**.

---

## Common Attack Scenario

Example vulnerable request:

```
GET /account?id=102
```

An attacker may try:

```
GET /account?id=103
GET /account?id=104
GET /account?id=105
```

If the server does not check permissions correctly, sensitive information may be exposed.

---

## Key Concepts Learned

### Broken Access Control

Access control mechanisms must verify that a user is authorized to access specific resources.

Failing to implement proper checks can allow unauthorized data access.

---

### Parameter Manipulation

Attackers often manipulate parameters in URLs, forms, or API requests to attempt unauthorized access.

Common parameters include:

- user IDs
- document IDs
- order numbers
- file references

---

### Importance of Server-Side Validation

Authorization checks must always be implemented **on the server side**.

Client-side restrictions can easily be bypassed by modifying requests.

---

## What I Learned

IDOR vulnerabilities are surprisingly common in web applications.

Even simple applications can expose sensitive data if access control checks are not properly implemented.

This room reinforced the importance of:

- validating user permissions
- protecting sensitive endpoints
- implementing strong authorization logic

---

## Platform

Practice completed on **TryHackMe**.

This repository documents my learning journey into **cybersecurity and penetration testing**.
