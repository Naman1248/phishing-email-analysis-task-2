# 📧 Phishing Email Analysis Report

## 🚨 Suspicious Email Sample

**From:** `security-alert@micr0soft-support.com`  
**To:** `myname@gmail.com`  
**Subject:** Urgent Action Required – Your Microsoft Account Has Been Locked  

---

**Email Body:**

> Dear user,  
>  
> We detected unusual activity on your Microsoft account. For your security, your access has been temporarily suspended.  
>  
> Please verify your identity by clicking the link below:  
> 👉 [https://micr0soft-support-verification.netlify.app](https://micr0soft-support-verification.netlify.app)  
>  
> If you do not verify your account within 24 hours, all access will be permanently revoked.  
>  
> Thanks,  
> Microsoft Security Team

---

## ⚠️ Phishing Indicators Found

1. **Spoofed Email Domain**  
   - `security-alert@micr0soft-support.com` mimics Microsoft but uses “micr0soft” (zero instead of 'o') – a classic spoofing tactic.

2. **Urgent or Threatening Language**  
   - Subject line and message use pressure tactics: “Urgent Action Required”, “your access has been suspended”, and “permanently revoked”.

3. **Suspicious Link**  
   - The URL points to a fake Netlify site, not a legitimate Microsoft domain. Hovering over the link reveals the mismatch.

4. **Spelling / Grammar Issues**  
   - Awkward repetition: “For your security, your access...” and robotic tone. Lack of personalization also signals a bulk phishing attempt.

5. **Generic Greeting**  
   - “Dear user” instead of using the recipient’s real name suggests it’s a mass phishing attempt.

6. **Fake Branding**  
   - Although it claims to be from Microsoft, the domain and language indicate no official source.

7. **No Contact Info or Signature**  
   - Legitimate companies include phone numbers, physical addresses, or contact links – none are present.

8. **Missing Email Header Analysis**  
   - As headers are not provided, technical verification like DKIM, SPF, and Return-Path could not be performed. Normally, these help detect spoofing.

---

## 🛠 Tools & Techniques You Would Use (If Headers Were Present)

- **Google Admin Toolbox**
- **MXToolbox Header Analyzer**
- **Mailheader.org**
- Check SPF/DKIM authentication results
- Compare "From" vs. "Return-Path" headers

---

## 📚 Key Learnings

- Phishing emails rely on **urgency**, **fake domains**, and **social engineering**.
- Always inspect the sender’s email, verify links, and check for grammatical errors.
- Never click suspicious links — verify with the official website or security team.
