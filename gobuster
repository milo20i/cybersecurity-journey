# Gobuster – Web Enumeration Basics (TryHackMe)

This repository documents my hands-on practice with **Gobuster** during the TryHackMe room *Gobuster: The Basics*.

The goal of this lab was to learn how to enumerate:

* Directories
* DNS subdomains
* Virtual hosts (vhosts)

using the different modes of the Gobuster tool.

---

## 🔧 Tool Used

* **Gobuster** (v3.x)
* Wordlists from DirBuster

---

## 📌 Gobuster Modes Practiced

### 1️⃣ Directory Enumeration (dir mode)

Used to discover hidden directories and files on a web server.

Example command:

```
gobuster dir -u http://target.thm -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt
```

What I learned:

* How to identify valid directories
* How to handle servers returning non-standard status codes (e.g. 405)
* How to tune threads and timeouts

Result:

* Discovered multiple hidden directories
* Found flags through directory enumeration

---

### 2️⃣ DNS Enumeration (dns mode)

Used to enumerate subdomains of a target domain.

Example command:

```
gobuster dns -d offensivetools.thm -w subdomains.txt
```

What I learned:

* How DNS brute forcing works
* How to identify valid subdomains
* Importance of correct DNS configuration

Result:

* Identified multiple valid subdomains

---

### 3️⃣ Virtual Host Enumeration (vhost mode)

Used to discover virtual hosts configured on the same IP address.

Example command:

```
gobuster vhost -u http://offensivetools.thm -w subdomains.txt
```

What I learned:

* Difference between DNS and vhost enumeration
* How web servers route traffic based on Host headers

Result:

* Found active virtual hosts
* Retrieved additional flags via vhost discovery

---

## 🧠 Key Takeaways

* Gobuster is a powerful enumeration tool for web reconnaissance
* Different modes target different layers (directories, DNS, vhosts)
* Proper configuration is essential to avoid false positives
* Enumeration is a critical first step in web security assessments

---

## 🎯 Skills Practiced

* Web reconnaissance
* Directory brute forcing
* Subdomain enumeration
* Virtual host discovery
* Reading and interpreting scan results

---

## 🚀 Next Steps

* Combine Gobuster with tools like Nmap and Burp Suite
* Automate enumeration workflows
* Apply enumeration results in exploitation labs

---

*This repository is part of my hands-on cybersecurity learning journey on TryHackMe.*
