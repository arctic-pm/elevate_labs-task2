# 📊 Phishing Email Analysis Report

## 📌 Sample Overview

* **Type**: Phishing Email claiming to be from PayPal
* **Sender**: [support@paypa1.com](mailto:support@paypa1.com) (note the typo in domain)
* **Subject**: 🚨 Urgent: Your Account Has Been Suspended!
* **Fake URL**: [https://paypal-security-login-verification.com](https://paypal-security-login-verification.com)
* **Date**: 23 June 2025

---

## 🔍 Header Review

| Field         | Value                                                           |
| ------------- | --------------------------------------------------------------- |
| Return-Path   | [support@paypa1.com](mailto:support@paypa1.com)                 |
| Received From | mail.phishhost.ru (203.0.113.45)                                |
| SPF Check     | ❌ Failed                                                        |
| DKIM Check    | ❌ Failed                                                        |
| Reply-To      | [noreply@scamverifylogin.co](mailto:noreply@scamverifylogin.co) |
| Subject Line  | Urgent warning — account suspended                              |

**Observation**: The email originated from a suspicious server and fails key authentication checks, which strongly suggests spoofing.

📎 *See: `phishing-email-header.txt`*

---

## 🕵️ Content Inspection

### Red Flags Detected:

1. **Suspicious Email Domain**

   * The email comes from `paypa1.com` which closely imitates `paypal.com`.

2. **Threatening Language**

   * Phrases like *"Your account has been suspended"* are designed to create panic.

3. **Misleading Links**

   * Link text implies PayPal but redirects to a completely different domain.

4. **Odd Reply-To Address**

   * Any genuine support message would use an official PayPal domain, not `scamverifylogin.co`.

5. **No Personalization**

   * Starts with “Dear Customer” — a common trait of mass phishing emails.

6. **Tone and Style**

   * Generic language, unusual formatting, and a lack of branding raise concerns.

7. **Unfamiliar Sending Server**

   * Message is relayed through a server not linked to PayPal.

📸 *Screenshots attached: `email-analyse-result.png`, `email-analyse-result_2.png`*

---

## ✅ Summary Table

| Characteristic               | Found?   |
| ---------------------------- | -------- |
| Fake/Spoofed Email Domain    | ✅        |
| SPF or DKIM Failures         | ✅        |
| Urgent or Fear Tactics       | ✅        |
| Misleading Links             | ✅        |
| Unusual Reply-To Address     | ✅        |
| Lack of Personalization      | ✅        |
| Grammar or Formatting Issues | ⚠️ Minor |
| Unknown Mail Server          | ✅        |

---

## 📎 Supporting Files

* `phishing-email.txt`: Full content of the phishing email
* `phishing-email-header.txt`: Complete message header for analysis
* `email-analyse-result.png`: Screenshot of email body analysis
* `email-analyse-result_2.png`: Screenshot of suspicious link behavior
* `README.md`: Describes process and summary

---

## 🔐 Final Notes

This email exhibits all the hallmarks of a phishing attempt. The combination of spoofed domains, broken authentication, suspicious links, and manipulative language are typical techniques used by attackers. Avoid clicking any links, and report the message through your organization's official security channels.
