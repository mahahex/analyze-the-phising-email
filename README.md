# 🛡️ Phishing Email Analysis Project

## 📌 Task 2: Analyze a Phishing Email Sample

### 🎯 Objective
This project aims to identify phishing characteristics in a suspicious email and build awareness of phishing tactics and email threat analysis skills.

---

## 🧰 Tools Used
- 📧 Sample phishing email (sourced from PhishTank, security training datasets)
- 🛠️ [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- 💻 Email client (Gmail, Outlook, Yahoo, etc.) for viewing headers and content

---

## 📝 Step-by-Step Analysis

### 1. Sample Phishing Email
- **Subject:** `Your PayPal Account Is Suspended – Act Now!`
- **From:** `support@secure-paypal-login.com`
- **Claimed Source:** PayPal

### 2. Check the Sender’s Email Address
- The sender domain is fake (`secure-paypal-login.com`) and mimics the official domain (`paypal.com`).
- ✅ **Phishing Indicator:** Spoofed sender address.

### 3. Analyze Email Headers with MxToolbox
- **SPF Check:** ❌ Failed  
- **DKIM:** ❌ Not configured  
- **Return-Path:** Different from the sender address  
- **Sending IP:** Not associated with PayPal  
- ✅ **Phishing Indicator:** Fails technical authentication checks (SPF/DKIM).

### 4. Suspicious Links and Attachments
- **Link text:** `https://paypal.com/verify`  
- **Actual URL (hover):** `http://secure-login-paypalverify.net/verify`  
- **Attachment:** `verify-now.html`  
- ✅ **Phishing Indicator:** Mismatched links + suspicious file attachment.

### 5. Urgent/Threatening Language
> “Your account will be suspended if you don’t verify within 24 hours.”  
- ✅ **Phishing Indicator:** Tries to scare the recipient into fast action.

### 6. Grammar and Spelling Mistakes
- “Your account will be suspend.”
- “Click imediately to restore your acccount.”
- ✅ **Phishing Indicator:** Poor grammar is a common sign of phishing.

---

## ✅ Summary of Phishing Characteristics

| 🔍 Indicator              | 📋 Description                                       |
|---------------------------|------------------------------------------------------|
| Fake sender domain        | Uses lookalike domain (not paypal.com)              |
| Fails SPF/DKIM checks     | Sent from unauthorized server                       |
| Urgent tone               | Tries to create panic for fast action               |
| Mismatched URLs           | Link text and destination don’t match               |
| Suspicious attachment     | `.html` file may contain malicious code             |
| Spelling/grammar issues   | Multiple language errors present                    |

---

## 🛑 Conclusion

This email is a **phishing attempt**. It uses fake links, spoofed sender information, and urgency to try and trick the user into giving away sensitive data.

### 🚨 Recommended Actions:
- ❌ Do not click on links  
- ❌ Do not open attachments  
- 📩 Report the email as **Phishing** or **Spam** to IT or your provider

---

## 🧠 Outcome
- Gained hands-on experience with real phishing analysis  
- Learned to recognize key phishing signs (spoofed sender, fake links, scare tactics)  
- Practiced using email header tools for threat detection

---

> 🔐 Stay alert. Think before you click.

