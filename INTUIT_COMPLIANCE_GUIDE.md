# Intuit QuickBooks App Compliance Guide
## Completing Production Credential Requirements

---

## ✅ COMPLETED
- [x] Review Intuit Developer Portal Profile
- [x] Verify email address

---

## 📝 TO COMPLETE

### 2. End-User License Agreement (EULA)

**What Intuit Needs:** URL to publicly accessible EULA

**What to Do:**
1. Host `EULA.md` on a public URL (options below)
2. Enter that URL in the Intuit Developer Portal

**Hosting Options:**

**Option A: GitHub (Free & Easy)**
1. Create a public GitHub repository (or use existing)
2. Upload `EULA.md`
3. Get raw file URL: `https://raw.githubusercontent.com/YOUR-USERNAME/YOUR-REPO/main/EULA.md`
4. Or use GitHub Pages for a nicer format

**Option B: Your Company Website**
1. Upload to: `https://www.culinarycanvasstl.com/tripleseat-qbo-eula`
2. Make sure it's publicly accessible

**Option C: Google Docs (Quick)**
1. Upload EULA.md to Google Docs
2. Set sharing to "Anyone with the link can view"
3. Use the share link

**Recommended:** Use your company website for professionalism

---

### 3. Privacy Policy

**What Intuit Needs:** URL to publicly accessible Privacy Policy

**What to Do:**
1. Host `PRIVACY_POLICY.md` on same location as EULA
2. Enter URL in Intuit Developer Portal

**Suggested URLs:**
- `https://www.culinarycanvasstl.com/tripleseat-qbo-privacy`
- Or same hosting method as EULA

---

### 4. App's Host Domain, Launch URL, and Disconnect URL

**Host Domain:**
- Since this is a locally-installed Python application (not a web app), enter:
  ```
  localhost
  ```
  Or if you'll host it on a server:
  ```
  your-server-domain.com
  ```

**Launch URL:**
- For local Python app: Not applicable
- Enter: `http://localhost:8000` (the OAuth redirect URI)
- Or mark as "N/A - Desktop Application"

**Disconnect URL:**
- URL where users can disconnect/revoke access
- For local app: Not applicable
- Enter same as Launch URL or mark N/A
- Note: Users can disconnect via QuickBooks settings

**Explanation to Provide:**
```
This is a server-side Python application that runs locally on 
the user's computer or their internal server. It does not have 
a public web interface. Users authenticate via OAuth redirect 
to http://localhost:8000/callback. Users can disconnect the 
app through their QuickBooks account settings.
```

---

### 5. Select at Least One Category

**What to Select:**
- **Primary:** Accounting
- **Secondary:** CRM (Customer Relationship Management)
- **Or:** Point of Sale

**Recommended Selection:**
- ✅ Accounting (primary - creates invoices)
- ✅ CRM (manages customer data)

---

### 6. Regulated Industries

**Question:** "Does your app serve any regulated industries?"

**Answer:** NO

**Explanation:**
```
This application is an internal business tool for synchronizing 
event management data with accounting software. It does not 
serve healthcare, financial services, or other regulated industries.
```

---

### 7. Where is Your App Hosted?

**Question:** "Tell us where your app is hosted"

**Answer:** 
```
Self-hosted / On-premises

This is a Python application that runs on the customer's local 
computer or internal server. It is not hosted on any cloud 
platform. Each installation is independent and controlled by 
the customer.
```

**Additional Details:**
- **Cloud Provider:** None (self-hosted)
- **Data Storage:** Local SQLite database on customer's system
- **Data Transmission:** Direct API calls to QuickBooks and Tripleseat
- **No External Servers:** All data flows directly between customer's accounts

---

## 📄 FILES PROVIDED

I've created these documents for you:

1. **`EULA.md`** - Complete End-User License Agreement
2. **`PRIVACY_POLICY.md`** - Complete Privacy Policy

**Both documents include:**
- ✅ Standard legal protections
- ✅ Specific QuickBooks/Tripleseat integration details
- ✅ Data handling explanations
- ✅ User rights and responsibilities
- ✅ CCPA and GDPR compliance sections
- ✅ Your company contact information

---

## 🔗 HOSTING RECOMMENDATIONS

### Quick Solution (5 minutes)

**Use GitHub:**
1. Go to https://github.com
2. Create new repository: `tripleseat-qbo-integration`
3. Set to **Public**
4. Upload `EULA.md` and `PRIVACY_POLICY.md`
5. Get URLs:
   - EULA: `https://github.com/YOUR-USERNAME/tripleseat-qbo-integration/blob/main/EULA.md`
   - Privacy: `https://github.com/YOUR-USERNAME/tripleseat-qbo-integration/blob/main/PRIVACY_POLICY.md`

### Professional Solution (30 minutes)

**Add to Company Website:**
1. Convert .md files to HTML (I can help with this)
2. Upload to your website
3. URLs:
   - `https://www.culinarycanvasstl.com/apps/tripleseat-qbo/eula`
   - `https://www.culinarycanvasstl.com/apps/tripleseat-qbo/privacy`

---

## ✅ COMPLETION CHECKLIST

Once you have hosting URLs, enter in Intuit Portal:

- [ ] EULA URL: ____________________
- [ ] Privacy Policy URL: ____________________
- [ ] Host Domain: `localhost` or your server domain
- [ ] Launch URL: `http://localhost:8000` or N/A
- [ ] Disconnect URL: Same as Launch URL or N/A
- [ ] Category: Accounting, CRM
- [ ] Regulated Industries: NO
- [ ] App Hosting: Self-hosted/On-premises

---

## 📧 NEED HELP?

**Converting documents to HTML?** Let me know and I'll create HTML versions.

**Questions about any field?** I can provide more specific language for Intuit's forms.

**Ready to proceed?** Let me know when you've hosted the documents and I'll help with any remaining questions.

---

## ⏱️ TIMELINE

**Estimated Time to Complete:**
- Hosting documents: 5-30 minutes
- Filling out Intuit forms: 15-20 minutes
- **Total:** 20-50 minutes

**Intuit Review Time:**
- Typically 1-3 business days
- May request clarifications
- Be ready to respond promptly

---

## 🎯 AFTER APPROVAL

Once Intuit approves:
1. You'll get production API credentials
2. Update `config_production.json` with new credentials
3. Follow DEPLOYMENT_GUIDE.md for production setup
4. System will be ready to go live!

---

**Questions? Need any documents converted to HTML? Ready to proceed with hosting?**
