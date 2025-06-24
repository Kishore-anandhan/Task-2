## 📧 Phishing Email Analysis Report

### 📝 Objective
Identify and document phishing characteristics in a suspicious email using forensic techniques.

---

### 🛠️ Tools Used
- Email client or `.txt` file viewer
- [MxToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- VirusTotal (https://virustotal.com)
- Web browser (for inspecting link destinations)

---

### 📂 Sample Phishing Email (Safe Text Version)

From: PayPal Security Team support@paypa1.com

To: user@example.com

Subject: Urgent: Your PayPal Account Has Been Suspended

Dear Valued Customer,

We have detected unusual activity in your PayPal account and have temporarily suspended access for your protection.
To restore access, please verify your account information by clicking the link:
https://www.paypal.com.security-check-verify-user.com/login
Failure to confirm your identity within 24 hours will result in permanent account suspension.
Please do not reply to this message. This mailbox is not monitored.

Thank you,

PayPal Account Security Team

Attachment: Invoice_Statement.pdf.exe


---

### 🔍 Phishing Indicators Found

| Feature                         | Observation                                                                 |
|----------------------------------|------------------------------------------------------------------------------|
| Spoofed sender address           | `support@paypa1.com` – uses a fake domain with a “1” instead of “l”         |
| Header discrepancies             | Can be simulated; would show SPF/DKIM failure if tested                      |
| Urgency and threatening tone     | “Failure to confirm within 24 hours will result in suspension”              |
| Suspicious link                  | Appears to be PayPal, but domain is `security-check-verify-user.com`        |
| Attachment                       | `Invoice_Statement.pdf.exe` – executable file disguised as PDF              |
| Generic greeting                 | “Dear Valued Customer” instead of personalized greeting                     |
| Spelling/grammar issues          | Slight awkward structure in closing paragraph                               |

---

### ✅ Summary

This email displays multiple phishing traits, including a spoofed sender address, suspicious and mismatched link, malware disguised as an attachment, and urgent language designed to cause panic. This is a clear phishing attempt. Do **not** click on links or open attachments in such emails.
