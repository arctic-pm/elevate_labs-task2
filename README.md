# elevate_labs-task2
# 🛡️ Task 2: Phishing Email Analysis

## 🔍 Objective
 Identify phishing characteristics in a suspicious email sample.

---

## 📧 Sample Email Used
A realistic phishing email impersonating PayPal with spoofed sender and malicious link was used for this analysis.  
You can find the full email body in [`phishing-email.txt`](./phishing-email.txt).

---

## 🧪 Tools Used
- Online Email Header Analyzer: [MXToolbox](https://mxtoolbox.com/EmailHeaders.aspx)
- Manual inspection of:
  - Sender’s email
  - Reply-To headers
  - URLs and domains
  - Tone and grammar
  - SPF/DKIM/DMARC authentication

---

## 📌 Steps Followed

1. **Obtained** a phishing email sample (realistic example created for research).
2. **Examined** sender address for spoofing (used `paypa1.com` instead of `paypal.com`).
3. **Analyzed** email headers for SPF/DKIM/DMARC failures and sender path.
4. **Identified** a suspicious phishing link pretending to be a PayPal login page.
5. **Detected** urgency and fear-based language to prompt user action.
6. **Verified** mismatch between link text and actual destination URL.
7. **Reviewed** grammar and writing style for red flags.
8. **Summarized** all phishing indicators in a detailed report.

---

## 📂 Files in This Repo

| File Name | Description |
|-----------|-------------|
| `phishing-email.txt` | Full raw body of the phishing email |
| `phishing-analysis.md` | Complete technical analysis of phishing indicators |
| `README.md` | Overview of the task, methodology, and tools used |

---

## ✅ Outcome
The email shows strong evidence of phishing, including spoofed sender address, failed SPF/DKIM, mismatched URLs, and psychological manipulation tactics. It should be reported and deleted without clicking any links.

---
