# GOOGLE SEARCH CONSOLE SETUP CHECKLIST
**Website:** Mithilaipatti.in  
**Date:** June 3, 2026  
**Purpose:** SEO Monitoring, Indexing, Performance Tracking  

---

## PRE-SETUP REQUIREMENTS

### ✅ Prerequisites
- [x] Website deployed and live at https://mithilaipatti.in
- [x] robots.txt accessible at https://mithilaipatti.in/robots.txt
- [x] sitemap.xml accessible at https://mithilaipatti.in/sitemap.xml
- [x] HTTPS certificate installed and valid
- [x] All pages return HTTP 200 status
- [x] Canonical tags configured
- [x] Hreflang tags configured

---

## STEP-BY-STEP SETUP

### Step 1: Create Google Search Console Account

**If you don't have a Google account:**
- [ ] Go to https://accounts.google.com
- [ ] Click "Create account"
- [ ] Fill in required information
- [ ] Verify email address
- [ ] Complete setup

**If you already have a Google account:**
- [ ] Continue to next step

### Step 2: Access Google Search Console

- [ ] Go to https://search.google.com/search-console
- [ ] Click "Start Now" or "Sign In"
- [ ] Sign in with your Google account
- [ ] Accept the terms of service

### Step 3: Add Property

**Method 1: Add Domain (Recommended)**
- [ ] Click "Add Property" (top left)
- [ ] Select "Domain" tab
- [ ] Enter: `mithilaipatti.in` (without https://)
- [ ] Click "Continue"
- [ ] Choose verification method (see next step)

**Method 2: Add URL Prefix (Alternative)**
- [ ] Click "Add Property"
- [ ] Select "URL Prefix" tab
- [ ] Enter: `https://mithilaipatti.in`
- [ ] Click "Continue"
- [ ] Choose verification method

---

## PROPERTY VERIFICATION

### Verification Method 1: HTML Meta Tag (Easiest)

**In Google Search Console:**
- [ ] Copy the meta tag provided (e.g., `<meta name="google-site-verification"...>`)

**In index.html:**
- [ ] Open index.html
- [ ] Find the `<head>` section (around line 3-10)
- [ ] Paste the verification meta tag AFTER the canonical tag
- [ ] Save the file
- [ ] Deploy to GitHub Pages
- [ ] Wait 10 minutes
- [ ] Return to GSC and click "Verify"

### Verification Method 2: HTML File Upload (Alternative)

**In Google Search Console:**
- [ ] Download the verification HTML file

**On your server:**
- [ ] Upload the file to your website root directory
- [ ] Verify file is accessible at https://mithilaipatti.in/[filename].html
- [ ] Return to GSC and click "Verify"

### Verification Method 3: DNS Record (Advanced)

**If you have domain admin access:**
- [ ] Copy the TXT DNS record from GSC
- [ ] Go to your domain registrar (GoDaddy, Namecheap, etc.)
- [ ] Navigate to DNS settings
- [ ] Add the TXT record
- [ ] Wait up to 48 hours for propagation
- [ ] Return to GSC and click "Verify"

---

## POST-VERIFICATION SETUP

### Step 4: Submit Sitemap

**In Google Search Console:**
- [ ] Go to "Sitemaps" section (left menu)
- [ ] Click "Add/Test Sitemap"
- [ ] Enter: `sitemap.xml`
- [ ] Click "Submit"
- [ ] Verify sitemap appears in list with status "Success"

**Sitemap Details to Verify:**
- [ ] Entries detected: 5 (index + 3 pages + language variant)
- [ ] Status: "Success"
- [ ] Last read: Recent date
- [ ] Valid XML format

### Step 5: Configure Preferred Domain

- [ ] Go to Settings (gear icon → Settings)
- [ ] Look for "Preferred domain"
- [ ] Choose: `https://mithilaipatti.in/` (with HTTPS)
- [ ] Save changes

### Step 6: Verify Hreflang Configuration

- [ ] Go to "International Targeting" section
- [ ] Verify language variants are detected:
  - [ ] Tamil: https://mithilaipatti.in/?lang=ta
  - [ ] English: https://mithilaipatti.in/?lang=en
- [ ] Check for any errors or warnings

---

## REQUEST INDEXING

### Step 7: Request URL Inspection

**For Homepage:**
- [ ] Click "URL Inspection" tool (top search box)
- [ ] Enter: `https://mithilaipatti.in`
- [ ] Click "Inspect"
- [ ] Check status: "URL is on Google" or "Inspected URL"
- [ ] If not indexed, click "Request Indexing"

**For Policy Pages:**
- [ ] Repeat for:
  - [ ] https://mithilaipatti.in/privacy-policy.html
  - [ ] https://mithilaipatti.in/terms-conditions.html
  - [ ] https://mithilaipatti.in/about.html

---

## MONITORING & OPTIMIZATION

### Step 8: Monitor Coverage

**In Google Search Console:**
- [ ] Go to "Coverage" section
- [ ] Review indexed pages
- [ ] Check for any errors
- [ ] Resolve any crawl errors

**Expected Results:**
- [ ] Error: 0
- [ ] Valid with warnings: 0 (ideally)
- [ ] Valid: 5+ (homepage + pages + language variants)
- [ ] Excluded: 0 (ideally)

### Step 9: Monitor Performance

- [ ] Go to "Performance" section
- [ ] Set date range to last 3 months
- [ ] Monitor:
  - [ ] Clicks (CTR growth)
  - [ ] Impressions
  - [ ] Average position
  - [ ] Top queries
  - [ ] Top pages

**Target Metrics (Month 1):**
- Impressions: 50-200
- Clicks: 10-50
- CTR: 10-25%
- Avg Position: 20-40

### Step 10: Monitor Mobile Usability

- [ ] Go to "Mobile Usability"
- [ ] Check for issues:
  - [ ] Clickable elements too close: 0
  - [ ] Viewport not set: 0
  - [ ] Text too small: 0
- [ ] All issues resolved

**Expected Status:** ✅ No issues

---

## STRUCTURED DATA VERIFICATION

### Step 11: Validate JSON-LD Schemas

**In Google Search Console:**
- [ ] Go to "Enhancements" section (left menu)
- [ ] Look for "Rich Results" or "Structured Data"
- [ ] Check status of:
  - [ ] LocalBusiness schema
  - [ ] Place schema
  - [ ] WebSite schema

**Expected Results:**
- [ ] All schemas: "Valid"
- [ ] Errors: 0
- [ ] Warnings: 0

**If issues appear:**
- [ ] Use Rich Results Test: https://search.google.com/test/rich-results
- [ ] Copy JSON-LD code into tester
- [ ] Fix any validation errors
- [ ] Update index.html with corrections

---

## SECURITY & MANUAL ACTIONS

### Step 12: Check Security Issues

- [ ] Go to "Security Issues" section
- [ ] Verify: ✅ No security issues found
- [ ] If any appear:
  - [ ] Click issue to get details
  - [ ] Fix as recommended
  - [ ] Mark as fixed
  - [ ] Request review

### Step 13: Check Manual Actions

- [ ] Go to "Manual Actions" section
- [ ] Verify: ✅ No manual actions
- [ ] This indicates no Google penalty

---

## ADDITIONAL TOOLS & REPORTS

### Step 14: Set Up Additional Monitoring

**Link Reports:**
- [ ] Go to "Links"
- [ ] View top linking sites
- [ ] Monitor for quality backlinks

**Core Web Vitals:**
- [ ] Go to "Core Web Vitals"
- [ ] Monitor:
  - [ ] Largest Contentful Paint (LCP): <2.5s
  - [ ] First Input Delay (FID): <100ms
  - [ ] Cumulative Layout Shift (CLS): <0.1

**Page Experience:**
- [ ] Go to "Page Experience"
- [ ] Check:
  - [ ] Mobile-friendly: ✅
  - [ ] HTTPS: ✅
  - [ ] No intrusive interstitials: ✅
  - [ ] Core Web Vitals: Monitor

---

## FIRST WEEK MONITORING

### Day 1 (Setup Day)
- [ ] Property verified in GSC
- [ ] Sitemap submitted
- [ ] Homepage URL inspection completed
- [ ] All policy pages requested for indexing

### Day 2-3 (Initial Crawling)
- [ ] Homepage appears in URL Inspection with status
- [ ] Coverage shows initial indexed pages
- [ ] No crawl errors expected

### Day 4-7 (Indexing Phase)
- [ ] All pages indexed
- [ ] Coverage: 5+ valid URLs
- [ ] First impressions appearing (likely minimal)
- [ ] Rich results validating
- [ ] First clicks likely to appear

**Expected Timeline:**
- Hours 0-6: Property verification
- Hours 12-24: First crawling (Googlebot visits)
- Days 1-3: Page indexing
- Days 3-7: Rich results processing
- Week 2+: Rankings appear

---

## MONTHLY MAINTENANCE CHECKLIST

### Monthly Tasks:
- [ ] Review "Performance" section (CTR, impressions, clicks)
- [ ] Check "Coverage" for new errors
- [ ] Monitor "Mobile Usability"
- [ ] Review "Core Web Vitals"
- [ ] Check for new manual actions
- [ ] Update content if needed
- [ ] Submit any new pages
- [ ] Resubmit sitemap (automatic, but can be manual)

### Quarterly Tasks:
- [ ] Analyze top performing queries
- [ ] Identify low-performing keywords
- [ ] Plan content improvements
- [ ] Review backlink profile
- [ ] Monitor competitor rankings

---

## TROUBLESHOOTING

### Issue: Property not verifying
**Solution:**
- Verify meta tag is correctly placed in index.html
- Check for typos in verification code
- Wait 10 minutes and retry
- Try alternative verification method (DNS or file upload)
- Ensure file is publicly accessible

### Issue: Sitemap not submitting
**Solution:**
- Verify sitemap.xml is valid XML
- Check sitemap.xml is accessible at /sitemap.xml
- Verify URLs in sitemap are correct
- Check robots.txt includes sitemap reference
- Wait 24 hours and resubmit

### Issue: Pages not getting indexed
**Solution:**
- Verify pages return HTTP 200 status
- Check robots.txt not blocking pages
- Verify canonical tags are correct
- Check no noindex meta tags
- Use "Request Indexing" in URL Inspection
- Allow 2-7 days for indexing

### Issue: Crawl errors appearing
**Solution:**
- Go to "Coverage" and check error details
- Fix errors on website
- Request recrawl in GSC
- Monitor for error resolution

---

## GOOGLE SEARCH CONSOLE SETUP STATUS

**Setup Date:** June 3, 2026  
**Expected Completion:** June 3, 2026 (same day)  
**Verification Method:** HTML Meta Tag (recommended)  
**Est. Time to Verify:** 10-30 minutes  
**Est. Time to Index:** 3-7 days  

---

## QUICK REFERENCE

### Important URLs:
- **Google Search Console:** https://search.google.com/search-console
- **Rich Results Test:** https://search.google.com/test/rich-results
- **Mobile Friendly Test:** https://search.google.com/mobile-friendly
- **PageSpeed Insights:** https://pagespeed.web.dev

### Key Metrics to Monitor:
- **Impressions:** 50+ (first month)
- **Clicks:** 10+ (first month)
- **CTR:** 10%+
- **Average Position:** 20-40 (first month)
- **Page Speed:** <3 seconds
- **Mobile Usability:** 0 issues

### Key Pages:
- Homepage: https://mithilaipatti.in/
- Privacy Policy: https://mithilaipatti.in/privacy-policy.html
- Terms & Conditions: https://mithilaipatti.in/terms-conditions.html
- About: https://mithilaipatti.in/about.html

---

**Checklist Created:** June 3, 2026  
**Status:** ✅ READY FOR IMPLEMENTATION  
**Estimated Time Required:** 30 minutes  
**Priority:** HIGH (Do within 1 day of deployment)

