# GOOGLE_DORKING

Here is a complete beginner-to-advanced level note on **Google Dorking**, written in simple words and formatted in **Markdown (`.md`)** for direct use in your GitHub repository:

---

````markdown
# Google Dorking - Beginner to Advanced Guide

> A complete guide to mastering Google Dorking for ethical hacking and OSINT investigations.

---

## 📌 What is Google Dorking?

Google Dorking (also called Google Hacking) is a technique that uses **advanced search operators** in Google to find hidden information, vulnerable websites, sensitive data, login pages, etc.

Google is more powerful than people think — with the right queries, you can discover **publicly exposed data** that shouldn't be indexed.

---

## 🧑‍🎓 Who Can Use It?

- Cybersecurity professionals
- Ethical hackers
- OSINT (Open Source Intelligence) researchers
- Bug bounty hunters
- Investigative journalists
- Anyone interested in smart searching

---

## 🔰 Basic Google Search Operators

| Operator      | Usage Example              | Description                                      |
|---------------|----------------------------|--------------------------------------------------|
| `site:`       | `site:example.com`         | Search only within a specific site               |
| `intitle:`    | `intitle:"login"`          | Finds pages with specific words in the title     |
| `inurl:`      | `inurl:admin`              | Finds URLs that include the word "admin"         |
| `filetype:`   | `filetype:pdf`             | Searches for specific file types (pdf, xls, etc) |
| `ext:`        | `ext:docx`                 | Same as filetype                                 |
| `intext:`     | `intext:"confidential"`    | Searches for specific words in page content      |
| `cache:`      | `cache:example.com`        | Shows cached version of a webpage                |
| `related:`    | `related:example.com`      | Finds sites similar to the one given             |

---

## 🧪 Beginner Dorks (Safe to Try)

```text
site:gov.in filetype:pdf "confidential"
intitle:"index of" "backup"
filetype:xls inurl:"email"
inurl:"/admin/login" "username"
````

These queries find:

* Government PDFs marked confidential
* Open directory listings
* Excel files with email data
* Admin login pages

---

## ⚠️ Intermediate Dorks (Recon & Discovery)

```text
inurl:"wp-content/uploads" filetype:pdf
site:pastebin.com "password"
site:linkedin.com/in intitle:"CEO" "company name"
intitle:"Index of" "db_backup"
```

Useful for:

* Discovering file leaks on WordPress
* Public pastebins with sensitive info
* Gathering employee info from LinkedIn
* Finding backup databases

---

## 🚨 Advanced Dorks (For Ethical Hacking ONLY)

```text
inurl:wp-admin intitle:"login"
filetype:env "DB_PASSWORD"
intitle:"index of" ".git"
site:example.com intext:"sql syntax error"
```

These can expose:

* Admin login panels
* Exposed environment files (.env)
* Public .git folders (code leaks)
* SQL errors (for SQLi testing)

> 🔐 **Use responsibly. Never attack or exploit systems without permission.**

---

## 🛡️ How to Protect Your Website from Google Dorking?

* Use `robots.txt` to block sensitive directories from search engines
* Do not store sensitive files publicly
* Disable directory listing on web servers
* Remove or secure `.git`, `.env`, `.bak`, and other sensitive files
* Monitor what’s indexed using Google Search Console

---

## 🔍 OSINT Use Cases of Google Dorking

* Finding leaked credentials
* Discovering internal documents
* Mapping an organization’s digital footprint
* Tracking down exposed APIs or test environments

---

## 📚 Tools That Support Google Dorking

* [Google Hacking Database (GHDB)](https://www.exploit-db.com/google-hacking-database)
* [Shodan](https://shodan.io) (for device search)
* [Spiderfoot](https://www.spiderfoot.net/)
* [Recon-ng](https://github.com/lanmaster53/recon-ng)

---

## 🧠 Tips for Smart Google Dorking

* Combine multiple operators for precision:
  `site:example.com filetype:xls intext:"username"`
* Use quotes to search exact phrases
* Use minus sign `-` to exclude terms
* Regularly check GHDB for latest dorks
* Use with VPN or private window if you do frequent searches

---

## 🧑‍⚖️ Legal & Ethical Notice

> Google Dorking is **NOT illegal**, but using it to **access, exploit, or misuse data without permission is ILLEGAL.**
>
> Always get permission before testing or scraping data.

---

## ✅ Conclusion

Google Dorking is a powerful technique when used correctly. It can help you:

* Improve your OSINT skills
* Strengthen web application security
* Gather useful intelligence

Learn it, use it ethically, and teach others how to **defend** against it.

---

## 📎 Resources

* 🔗 [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)
* 📘 [OSINT Framework](https://osintframework.com)
* 📺 YouTube: Google Dorking tutorials
* 🧑‍🏫 OWASP Resources on OSINT & Recon



