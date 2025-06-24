# 📄 Phishing Email Analysis Report

## 🔍 Email Summary
- **Subject:** Your Account Has Been Locked – Immediate Action Required  
- **Sender:** "PayPal Security Team" <support@secure-acc0unt.com>  
- **Phishing URL:** [http://www.alert.scan001.com/error73oaB4-0983](http://www.alert.scan001.com/error73oaB4-0983)

---

## 📬 Header Red Flags (From header_analysis.txt)
- ❌ **SPF Validation:** Fail – domain `secure-acc0unt.com` does not authorize sending IP `185.31.210.99`
- ❌ **DKIM Signature:** Not found – no signature present
- ❌ **DMARC:** No DMARC policy found for the sender domain
- ❗ **Return-Path vs From Mismatch:** Sender claims to be PayPal, but domain is `secure-acc0unt.com`
- 🛑 **Suspicious IP:** Email relayed from unknownserver.host.com (IP not blacklisted but untrustworthy)

---

## 🔗 Link and Domain Spoofing
- **Displayed Link:** Claims to be from PayPal
- **Actual Link:** `http://www.alert.scan001.com/error73oaB4-0983`
- **Analysis:** This link does not belong to PayPal and likely leads to a phishing website designed to steal login credentials or sensitive information.

---

## 🧠 Language and Tone Indicators
- **Urgency:** Uses scare tactics — “Your account has been locked”
- **Action Pressure:** Demands “immediate action”
- **Emotional Trigger:** Threat of account lockout creates panic and fear

---

## ✏️ Spelling and Grammar Errors
- The domain name `secure-acc0unt.com` uses a **zero (0)** in place of an **o**, which is a common phishing trick
- Grammar is mostly formal but content tone is over-aggressive and not standard for verified PayPal communication

---

## ✅ Conclusion
This email is a **clear phishing attempt**:
- It impersonates a trusted brand (PayPal)
- Fails all authentication checks (SPF, DKIM, DMARC)
- Contains a spoofed link to an external domain
- Tries to exploit user urgency and fear

📌 **Recommendation:** Do NOT click links or reply. Mark as spam and report to your IT/security team or the impersonated company.

---

## 📁 Files Used in This Analysis
- `Phishing email sample.txt`
- `header_analysis.txt`

✅ Add this report as `phishing_report.md` to your GitHub repo under `phishing-email-analysis/`

