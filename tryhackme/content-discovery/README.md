# Content Discovery — TryHackMe

## Overview

This lab focuses on **Content Discovery**, a key technique used during the **reconnaissance phase of a penetration test**.

The goal is to identify hidden files, directories, and endpoints on a web server that are not directly accessible through the website navigation.

Discovering hidden content can reveal:

- Admin panels
- Backup files
- Configuration files
- Sensitive endpoints

---

## Tools Used

During this room I practiced using common enumeration tools:

- Gobuster
- Dirsearch
- Wordlists

These tools automate the process of testing thousands of possible directories and files.

---

## Example Command

Example of directory brute forcing with **Gobuster**:

```bash
gobuster dir -u http://target-site.com -w /usr/share/wordlists/dirb/common.txt
