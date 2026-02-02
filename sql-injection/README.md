# SQL Injection

This section documents my hands-on learning and practice related to **SQL Injection**, one of the most critical vulnerabilities listed in the **OWASP Top 10**.

The goal of this lab is to understand:
- How SQL Injection vulnerabilities occur
- How attackers exploit insecure input handling
- How to prevent SQL Injection using secure coding practices

---

## 🔍 What is SQL Injection?

SQL Injection is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database.  
It usually occurs when user input is directly concatenated into SQL queries without proper validation or parameterization.

---

## 🧪 Practical Overview

In this exercise, I:
- Identified vulnerable input fields
- Tested user input for SQL Injection
- Exploited the vulnerability to bypass authentication and/or extract data
- Analyzed the root cause of the issue

> ⚠️ All activities were performed in a **legal and controlled lab environment** (TryHackMe).

---

## 🛡️ Mitigation Techniques

Some effective defenses against SQL Injection include:
- Using **prepared statements / parameterized queries**
- Input validation and sanitization
- Applying the principle of **least privilege** for database users
- Avoiding dynamic SQL construction

---

## 🧠 Skills Practiced

- Web Application Security
- OWASP Top 10
- SQL Injection techniques
- Secure coding principles
- Secure coding best practices

---

## 📌 Notes

This repository is part of my **cybersecurity learning journey**, focused on building both offensive and defensive security skills.
