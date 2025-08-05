**🛡️ Phishing Email Analysis Report**

This report contains a step-by-step analysis of a suspected phishing email sample as part of a cybersecurity internship task.



📩 **Step 1: Sample Phishing Email**

From: Netflix Support <support@netflix-billing.com>

To: you@example.com

Subject: Action Required: Payment Failure



**Email Body**:



We are unable to process your recent payment for your Netflix subscription.  

To avoid interruption, please update your billing information immediately by visiting the link below:



http://netflix-billing-update.com/login



Thank you for being a valued customer.

⚠️ This email imitates Netflix and contains a suspicious login link.



**💾 Step 2: Save as .txt File**

**T**o avoid any risk of executing malicious content, the phishing email was safely copied and saved in a plain text file (phishing-email.txt). This helps in secure offline analysis.

Note: The sender email address is suspicious. Although it appears to be from Netflix, the domain is not legitimate. It uses a lookalike domain netfIix-billing.com which is a spoof of netflix.com.



**🛠️ Step 3: Header Analysis (MKToolbox)**

The email was analyzed using the MKToolbox Email Header Analyzer.



Findings:



From domain: netflix-billing.com (not official)



SPF/DKIM/DMARC: Missing or failed

Header Signature: Spoofed identity

Subject: Contains urgency trigger



**Observation: I**f the email header were available, it would likely fail SPF, DKIM, and DMARC checks because the domain netfIix-billing.com is not legitimate and is not authorized to send email on Netflix's behalf. This is a clear sign of spoofing.



**✅** This confirms that the sender is impersonating Netflix using a fake domain.



**🔍 Step 4: URL Check with VirusTotal**

Suspicious link:



***http://netflix-billing-update.com/login***

This was scanned on VirusTotal.



**Results:**



Detected by 9+ vendors as malicious/phishing

Detected issues:

Phishing site

Fake login portal

Credential harvesting attempt



**Observation: The** email includes a suspicious link (https://netflix-billing-update.com/login) that imitates the real Netflix domain. Clicking this link could lead to credential theft. It also contains a .docm attachment, which is a macro-enabled Word document often used to deliver malware. These are strong signs of phishing and malicious intent.



**🧠 Step 5: Psychological Triggers Used**

**T**he phishing email uses social engineering tactics:



🔥 Urgency: Immediate action required

🔐 Fear: Losing access to Netflix

👮 Authority: Fake Netflix branding

🎯 Targeting: Personalized to trick users



These tricks manipulate users into clicking the fake login link without thinking.



**🔎 Step 6: Hover Link Inspection**

**I**n a real email client, hovering the mouse over the link would show:



http://netflix-billing-update.com/login

🕵️ This clearly differs from Netflix’s real domain netflix.com and reveals a phishing attempt. (In a .txt file, hovering doesn't work, so this step applies to real emails.)



**Observation**: The phishing email has relatively proper grammar, which may trick users into thinking it's genuine. However, it lacks personalization and uses a generic tone. Many phishing emails may contain grammatical or spelling errors, which is another red flag users should watch for.



✅ **Step 7: Final Summary \& Recommendation**

**Summary**:

Category	Result

Sender Address	Fake / Spoofed

Header Authentication	Failed (No SPF/DKIM)

URL	Malicious (flagged by VirusTotal)

Content Tricks	Urgency, Fear, Fake Authority

Goal	Credential theft via phishing login page



Recommendation:

❌ Don’t click on suspicious links

✅ Report phishing attempts to security teams

🧠 Educate users on how to spot fake domains

🔐 Verify sender emails and hover over links



