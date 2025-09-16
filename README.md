# HivePass – Team Credential Vault (Browser Extension)

> **TL;DR**: HivePass lets developers and QA securely share **project‑specific website credentials** right from the browser. One teammate saves creds once; everyone on the project can use them—no more pinging people for logins. **Do not store personal emails** here, and **company email accounts are blocked** by design.

---

## ✨ What is HivePass?

HivePass is a lightweight browser extension for internal testing environments. It stores and auto‑fills **non‑personal** credentials for websites under development at your IT firm, so devs/testers don’t have to ask around for access.

---

## 🚀 Core Features

* **Project‑scoped credentials**: Save creds per domain/app (e.g., `staging.example.com`).
* **Shared access**: Teammates on the same project instantly get read‑only access.
* **One‑click autofill**: Fill username/password on supported login forms.
* **Role‑aware visibility**: Owners can edit; collaborators consume.
* **Audit trail**: Who created/updated a credential and when.
* **Zero personal emails**: Personal email addresses are disallowed; company email logins are blocked.
* **Encrypted at rest & in transit**: Keys managed by the org; only authorized members can decrypt.

> **Not for production customer data.** HivePass is intended for **internal test/stage** environments only.

---

## 🧩 How It Works

1. **Install** the extension and sign in with your org account.
2. Navigate to a test/stage URL (e.g., `https://staging.yourapp.com`).
3. Click **HivePass → Add Credential**.
4. Enter **Username** + **Password** (personal/company emails are not allowed).
5. Choose **Project** and optional **Tags** (e.g., `qa`, `smoke`, `admin-user`).
6. Save → the record syncs to your project.
7. Teammates visiting the same site see **Use Credential** → **Autofill**.

---
### Install HivePass Extension

\:white\_check\_mark: **For Chrome:**

1. Go to: `chrome://extensions/`
2. Enable **Developer Mode** (top right).
3. Click **Load unpacked**.
4. Select the `chrome` folder from the extracted HivePass files.
5. You will now see HivePass in the extension list.

\:white\_check\_mark: **For Edge:**

1. Go to: `edge://extensions/`
2. Enable **Developer Mode** (left side).
3. Click **Load unpacked**.
4. Select the `chrome` folder from the extracted HivePass files.
5. You will now see HivePass in the extension list.

\:white\_check\_mark: **For Firefox:**

1. Go to: `about:debugging#/runtime/this-firefox`
2. Click **Load Temporary Add-on**.
3. Select the `manifest.json` file from the `firefox` folder.
4. HivePass will now appear in your extension list.

\:warning: **Note:** You must be logged in at [https://pms.softwareco.com](https://pms.softwareco.com) for the extension to work properly.

---


## ✅ Do / ❌ Don’t

**Do**

* Store only test/stage credentials.
* Use generic test usernames (no emails).
* Tag entries for clarity.

**Don’t**

* ❌ Store **personal emails** as usernames.
* ❌ Store **company email accounts**—HivePass blocks these.
* ❌ Put production/customer secrets.

* `1.0.0` – Initial release: shared creds, autofill.
