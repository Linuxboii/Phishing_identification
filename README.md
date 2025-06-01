# Phishing Email Analysis – Task 2

## Objective
Analyze a suspicious email and identify phishing indicators to better understand common email-based cyber threats.

## Tool Used
mxtoolbox.com - Greatly helped in analysing the email header.

## Sample Email Analyzed
The email pretended to be from Apple Security and used fear tactics to convince the user to click a malicious link.

### Key Details:
- **Sender:** security@apple-id-update.com
- **Subject:** URGENT: Your Apple ID Has Been Suspended
- **Malicious Link:** https://apple.com.verify-user-login.com/restore
- **Attachment:** Account_Recovery.pdf (suspected malicious)
- **Greeting:** "Dear Customer" (generic)
- **Urgency:** “Verify within 24 hours or get suspended”

---

## Phishing Indicators Found
| Indicator | Description |
|----------|-------------|
| 🚩 Spoofed Email | The domain is not official Apple (`apple-id-update.com`) |
| 🚩 Suspicious Link | Link masks itself as Apple but redirects to a phishing domain |
| 🚩 Urgent Language | Threatens suspension if user doesn't act quickly |
| 🚩 Failed Header Checks | SPF, DKIM, and DMARC all failed |
| 🚩 Generic Greeting | Doesn't mention user’s real name |
| 🚩 Unusual Attachment | PDF file not expected from Apple |

