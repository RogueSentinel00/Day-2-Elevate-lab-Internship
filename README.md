# Day-2-Elevate-lab-Internship

✅ Real-World Phishing Email Example: "Your PayPal Account Is Limited"

📧 Email Details

Subject: "Your PayPal account has been limited due to suspicious activity"
From: service@paypa1.com
To: victim@example.com
Date: June 2025

 Email :

Dear Customer,

We’ve noticed unusual activity in your PayPal account and have temporarily limited it for your protection.

To restore full access, please verify your information immediately.

Failure to do so within 24 hours will result in permanent suspension.

Click here to verify your account:

https://paypal.com.secure-authentication-center.com/login

Thank you,
PayPal Security Team

🔍 Phishing Analysis


1. Examine Sender's Email Address for Spoofing
From: service@paypa1.com

Appears close to the legitimate paypal.com.

The "1" replaces "l" — a common spoofing tactic.

✅ Spoofed domain detected (paypa1.com ≠ paypal.com).

2. Check Email Headers for Discrepancies
Using tools like MXToolbox Analyzer:

SPF/DKIM/DMARC authentication fails.

Return-Path doesn't match the "From" address.

Email was sent from an IP not associated with PayPal.

✅ Header inconsistencies found.

3. Identify Suspicious Links or Attachments
Link: https://paypal.com.secure-authentication-center.com/login

At first glance, it looks legitimate.

But the actual domain is secure-authentication-center.com — not PayPal.

It’s a credential harvesting site.

✅ Malicious link identified.

4. Look for Urgent or Threatening Language
“Failure to do so within 24 hours will result in permanent suspension.”

Designed to pressure the victim into acting quickly without thinking.

✅ Urgency and threat present.

5. Note Any Mismatched URLs
Hover over:

“Click here to verify your account” → reveals
https://paypal.com.secure-authentication-center.com/login

This is not PayPal; it’s a fake login page.

✅ Mismatched and deceptive URL confirmed.

6. Verify Presence of Spelling or Grammar Errors
“Failure to do so within 24 hours will result in permanent suspension.”

Mostly grammatically correct, but formal tone seems slightly robotic.

Other phishing emails may have more obvious issues.


Summarize Phishing Traits Found in the Email
Trait	Status	Details
Spoofed sender address	✅	paypa1.com mimics PayPal
Header discrepancies	✅	SPF/DKIM fail, suspicious IP and return-path
Suspicious link	✅	Fake PayPal site using a misleading domain
Urgent/threatening tone	✅	“24 hours” and “permanent suspension” used as pressure
Mismatched link	✅	Hover reveals it’s not going to paypal.com
Spelling/grammar issues	⚠️	Slightly odd tone, no major grammar errors

🧠 Conclusion
This phishing email impersonates PayPal with:

A spoofed domain (paypa1.com)

A fake urgent issue (account suspension)

A misleading URL that appears to be PayPal

A fake link that collects credentials
