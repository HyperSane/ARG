---
color: var(--mk-color-blue)
sticker: emoji//1f579-fe0f
Publish: true
Obsidian-Type:
  - Guide
Title:
  - GPG Basic Guide
Related-To:
  - Encryption
  - ARG Layers
Type:
  - Guide
  - Encryption
Types:
  - ARG-Core
  - Hyper-Sanity
  - ARG-Guide
tags:
  - ARG-Guide
Date-Created: 2025-04-07
last-updated: ""
Favorite: 
Date: ""
Path:
  - ARG\ARG Guides\Encryption
Origin:
  - HyperSane Demon
ARG: false
TODO: 
Project: 
Project-Folder: 
Template:
  - ARG1-4 Manual
GPT-Title:
  - ""
GPT-Links:
  - "[[]]"
GPT-URL: 
GPT: 
Ethics: 
MetaPhysic: 
Links:
  - ""
Canvas-Link:
  - Symbolic_Map.canvas
Scripts:
  - "last-updated: <% tp.user.update_last_updated(tp) %>"
  - "auto-tagging: <% tp.user.auto_tagging(tp) %>"
  - "correlation-check: <% tp.user.correlation_check(tp) %>"
  - "project-folder-sync: <% tp.user.project_folder_sync(tp) %>"
BackLinks: 
ForwardLinks: 
Reddit:
  - ""
Attachments:
  - ""
Exerpt: 
Keywords: 
MetaData:
  - HyperSane Demon
  - HyperSanityARG
Wikipedia:
  - https://en.wikipedia.org/wiki/GNU_Privacy_Guard
Length:
---



created: 2025-03-31
---

# 🛡️ How to Decrypt Encrypted ARG Drops Using GPG

This guide teaches you how to decrypt `.gpg` files found throughout the ARG using free tools. You'll only need a basic understanding of file handling and a passphrase (hidden within the ARG).

> **Encrypted drops** protect secrets using AES256 encryption and a password (not a keypair). You do not need to create an account or upload anything.

---

## 🔧 Tools You Need

| Platform | Tool                | Download Link                          |
|----------|---------------------|----------------------------------------|
| Windows  | Gpg4win (Kleopatra) | https://gpg4win.org/                   |
| macOS    | GPGTools            | https://gpgtools.org/                  |
| Linux    | GnuPG (built-in)    | Already installed or `sudo apt install gnupg` |

---

## ✅ How to Decrypt a Drop (Quick Version)

1. Download the `.gpg` file from the ARG (e.g., from GitHub).
2. Open Kleopatra (or GPGTools on Mac).
3. Click **File > Decrypt/Verify**.
4. Choose the `.gpg` file.
5. When prompted, enter the **passphrase** you found in the ARG.
6. The decrypted file will appear in your downloads folder or be saved alongside the original.

---

## 🔐 Decrypt Using Terminal (Optional)

```bash
gpg -d EncryptedDrop.gpg -o DecryptedOutput.pdf
```
Then enter the password when prompted.

---

## 🔎 Where to Find the Passphrase?

Passphrases are hidden in:
- ARG puzzles and riddles
- Embedded messages or timestamps
- Fragments of quotes or repeated numbers

> Example: If the riddle says “thrice repeated truth,” the code might be `369369369`.

---

## 🧠 Frequently Asked Questions

### What is `.gpg`?
It's a file encrypted using the GPG (GNU Privacy Guard) system — typically using AES256 if protected by a password.

### Do I need a key?
No. ARG drops use **symmetric encryption** — you only need a password.

### Is it safe?
Yes. Decryption happens **locally** on your machine. Your data isn’t uploaded anywhere.

### I entered the password but it says "bad session key"
You likely mistyped the passphrase. Try again carefully.

---

## 🎯 Goal
These encrypted drops often contain:
- Hidden documents
- Unredacted archives
- Secret links or timeline clues

Decryption is your rite of passage.

---

If you run into trouble, ask in the ARG discussion threads. Otherwise: trust the code, and dive deeper.
