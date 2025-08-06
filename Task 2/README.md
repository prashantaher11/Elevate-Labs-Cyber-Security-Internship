# 📄 Phishing Email Investigation Report  
**Cyber Security Internship – Task 2**  
**Email Subject:** Action Required: Suspicious Activity Detected  
**Tool Used:** MXToolbox Header Analyzer  
**Date:** August 6, 2025

---

<img width="791" height="887" alt="Screenshot 2025-08-06 162025" src="https://github.com/user-attachments/assets/e8abce88-c296-4147-85d3-ac14c6c2b3bb" />

---

## 📬 1️⃣ Email Summary

| Field     | Details                                               |
|-----------|-------------------------------------------------------|
| **From**  | YourBank Security Team `<support@yourbank.secure-login.com>` |
| **To**    | John Doe `<johndoe123@gmail.com>`                     |
| **Date**  | Tue, 5 Aug 2025 10:24:32 +0530                        |
| **Subject** | Action Required: Suspicious Activity Detected       |

---

## 📌 2️⃣ Email Content & Visual Red Flags

| # | Indicator              | Explanation |
|---|------------------------|-------------|
| 1 | **Spoofed Sender Domain** | Claims to be from YourBank, but domain is `secure-login.com` — a fake, lookalike domain. |
| 2 | **No Personalization** | Uses generic "Dear Customer" instead of the user's real name. |
| 3 | **Urgency & Threat**   | Mentions "verify within 24 hours" to cause panic and trick user. |
| 4 | **Phishing Button**    | “Verify Your Account” button likely redirects to a phishing website. |
| 5 | **Grammatical Errors** | Mistakes like "att empts", "tem porarily" indicate poor quality. |
| 6 | **Fake Branding**      | Generic bank logo used, not consistent with official branding. |

---

## 🧪 3️⃣ Email Header Analysis (MXToolbox)

### ✉️ Header Fields Extracted

| Header Field | Value |
|--------------|-------|
| **From**     | YourBank Security Team `<support@yourbank.secure-login.com>` |
| **To**       | John Doe `<johndoe123@gmail.com>` |
| **Date**     | Tue, 5 Aug 2025 10:24:32 +0530     |
| **Subject**  | Action Required: Suspicious Activity Detected |

---

### 🖼️ Header Analysis Screenshots


<img width="1892" height="865" alt="Screenshot 2025-08-06 164037" src="https://github.com/user-attachments/assets/8f53e864-cf2b-42d9-a24b-a685a23e2b64" />

<img width="1890" height="873" alt="Screenshot 2025-08-06 164054" src="https://github.com/user-attachments/assets/5dddba86-889e-4fd2-9d25-9d78519225e8" />

---

### ⚠️ Technical Indicators of Spoofing

| Evidence | Explanation |
|----------|-------------|
| ❌ **No SPF/DKIM/DMARC Results** | Email lacks authentication — likely spoofed. |
| ❌ **Unverified Domain**         | `secure-login.com` is not owned by YourBank. |
| ❓ **No IP Origin Info**         | Missing details prevent traceability. |
| ✅ **Header Present**            | Basic headers found, but spoofers often manipulate them. |

---

## 🧠 🔐 How We Know It's a Spoofed Email

| Technique Used     | Result |
|--------------------|--------|
| ✅ Visual Inspection | Mismatched domain, fake urgency, layout issues |
| ✅ Header Analysis   | Lacks proper authentication (SPF, DKIM, DMARC) |
| ✅ Branding Check    | Generic logo used, no consistency with official design |
| ✅ Link Behavior     | Button likely leads to phishing site |
| ✅ Grammar Review    | Spacing and typo issues common in fake emails |

---

## ✅ Summary of Phishing Traits

- 📛 **Spoofed sender domain**
- 🚨 **Urgent language to scare the user**
- 👤 **Generic greeting ("Dear Customer")**
- 🏦 **Fake bank branding and logos**
- 🔗 **Credential harvesting link**
- 🛑 **Missing authentication headers (SPF, DKIM, DMARC)**

---

## 📂 Files Included (for GitHub)

