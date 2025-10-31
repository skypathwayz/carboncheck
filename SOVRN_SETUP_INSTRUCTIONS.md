# Sovrn Setup Instructions for CarbonChecks

## ✅ Your Sovrn Link Confirmed
**Your Amazon Sovrn link:** `https://sovrn.co/tb8n0h3`

This means Sovrn is working! Now you need to implement it.

---

## 🎯 TWO WAYS TO USE YOUR SOVRN LINK

### OPTION 1: Automatic Link Conversion (If Sovrn Provides Script)

**Best for:** Automatic tracking of ALL Amazon links

1. **Check Sovrn Dashboard for:**
   - "Integration" or "Site Setup" section
   - Look for JavaScript code/snippet
   - Copy the code they provide

2. **Add to Your Site:**
   - Paste Sovrn script before `</body>` tag in `index.html`
   - This will automatically convert all Amazon links

3. **Test:**
   - Visit your live site
   - Inspect an Amazon link
   - Should show Sovrn tracking URL

---

### OPTION 2: Manual Link Replacement

**Best for:** Precise control and guaranteed tracking

**How Sovrn Links Work:**
Your Sovrn link `https://sovrn.co/tb8n0h3` redirects to Amazon. 

**Format Options:**

**A) If Sovrn supports URL parameters:**
```
https://sovrn.co/tb8n0h3?url=https://www.amazon.com/s?k=solar+panel+kits
```

**B) If Sovrn uses the base link:**
- Replace all Amazon links with: `https://sovrn.co/tb8n0h3`
- Users click → Sovrn redirects → Amazon (with your tracking)

**C) Country-Specific Setup:**
Based on [Sovrn's documentation](https://www.sovrn.com/blog/amazon-tag-manager/), you need to:
1. Go to Sovrn Commerce → Affiliate Networks
2. Add Amazon Associates for each country:
   - US: Your US Amazon Associates tag
   - UK: Your UK Amazon Associates tag  
   - CA: Your Canadian Amazon Associates tag
   - AU: Your Australian Amazon Associates tag
   - DE: Your German Amazon Associates tag

3. Sovrn will generate country-specific links automatically

---

## 📋 WHAT TO DO NOW:

### Step 1: Check Sovrn Dashboard
- Look for "Integration" or "Site Code" section
- See if they provide automatic link conversion script
- If yes → Use Option 1
- If no → Use Option 2

### Step 2: Set Up Amazon Associates Tags
According to [Sovrn's Amazon Tag Manager](https://www.sovrn.com/blog/amazon-tag-manager/):
1. Go to Sovrn Commerce → Affiliate Networks
2. Select "Amazon Associates"
3. Add your tracking IDs for each country:
   - US (amazon.com)
   - UK (amazon.co.uk) 
   - CA (amazon.ca)
   - AU (amazon.com.au)
   - DE (amazon.de)

### Step 3: Test
1. Visit your live site
2. Click an Amazon link
3. Check if it redirects through `sovrn.co`
4. Check Sovrn dashboard for tracked clicks

---

## 🔧 IMPLEMENTATION OPTIONS

### If Sovrn Provides Auto-Conversion Script:
```html
<!-- Add before </body> tag -->
<script>
  // Sovrn provided code here
</script>
```

### If Manual Replacement Needed:
Replace Amazon links from:
```html
https://www.amazon.com/s?k=solar+panel+kits
```

To Sovrn format (check Sovrn dashboard for exact format):
```html
https://sovrn.co/tb8n0h3?url=https://www.amazon.com/s?k=solar+panel+kits
```

---

## ⚠️ IMPORTANT NOTES

1. **Geo-Targeting:** After adding Amazon Associates tags for each country in Sovrn, links should auto-convert based on user location

2. **Testing:** Always test on live site to confirm links work

3. **Dashboard:** Check Sovrn dashboard 24-48 hours after implementation to see tracked clicks

4. **Existing Links:** All current Amazon links on your site will need to be converted - either automatically via script OR manually replaced

---

**Your Current Sovrn Link:** `https://sovrn.co/tb8n0h3`
**Next Step:** Check Sovrn dashboard for integration code or manual link format

