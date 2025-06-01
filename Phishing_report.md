# Phishing Email Report

## Email Overview

**Subject:** URGENT: Your Apple ID Has Been Suspended  
**From:** security@apple-id-update.com  
**To:** you@example.com  
**Date:** Tue, 28 May 2025 14:32:11 +0000  
**Attachment:** Account_Recovery.pdf  
**Suspicious Link:** https://apple.com.verify-user-login.com/restore

---

## Header Analysis

| Field | Status |
|-------|--------|
| SPF | ❌ Softfail |
| DKIM | ❌ Failed |
| DMARC | ❌ Failed |
| Return-Path | notice@apple-id-update.com |
| Source IP | 185.99.100.45 (unverified domain) |
| Message-ID | APPLEID20250528143211@smtp7.apple-id-update.com |

Header analysis was performed using [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx).

---

## Phishing Indicators

| Indicator | Description |
|----------|-------------|
| 🛑 **Spoofed Sender** | The sender domain is not `apple.com`, it’s `apple-id-update.com`, which is a phishing lookalike. |
| 🛑 **Failed Authentication** | SPF, DKIM, and DMARC all failed, showing the email likely came from an untrusted source. |
| 🛑 **Urgent Tone** | The message uses fear tactics: “Your account is suspended” and “verify in 24 hours”. |
| 🛑 **Malicious Link** | The link looks legit at first glance but actually leads to a phishing site: `verify-user-login.com`. |
| 🛑 **Generic Greeting** | Uses "Dear Customer" instead of addressing the user by name. |
| 🛑 **Unexpected Attachment** | A PDF attachment pretending to be an “account recovery” document – typical phishing behavior. |

---

## Summary

This email is a textbook phishing attempt designed to steal Apple ID credentials by tricking the user into clicking a fake login link. The use of spoofed domains, urgency, and failed authentication headers makes it highly suspicious and dangerous.

> ⚠️ **Conclusion:** Do **NOT** click any links or download attachments. Report immediately to IT or your email provider.

