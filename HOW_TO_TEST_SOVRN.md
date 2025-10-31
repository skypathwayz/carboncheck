# How to Test if Sovrn Domain-Level Tracking Works

## 🧪 STEP-BY-STEP TESTING METHOD

### Method 1: Quick URL Test (Easiest)

1. **Add base domain to Sovrn:**
   - Go to Sovrn dashboard
   - Add `amazon.com` as a merchant/domain
   - Wait for approval (if needed)

2. **Check if Sovrn provides a script/code:**
   - Look for "Site Setup" or "Integration" in Sovrn dashboard
   - Sovrn might require you to add a JavaScript snippet to your site
   - If they provide a script, add it to your `index.html` (before `</body>` tag)

3. **Test the links on your live site:**
   - Visit your website (carbonchecks.com)
   - Right-click on ANY Amazon link (e.g., "Shop Solar Panels →")
   - Select "Copy Link Address" or "Inspect Element"
   - **If it works:** The URL will be converted to a Sovrn tracking link (will contain Sovrn domain like `sovrn.com`, `viglink.com`, or similar tracking parameters)
   - **If it doesn't work:** The URL will still be the original Amazon link

### Method 2: Browser Developer Tools Test

1. **Open your website in browser**
2. **Right-click on an Amazon link** → "Inspect" or "Inspect Element"
3. **Check the `href` attribute:**
   - **Working:** Will show something like:
     ```
     https://sovrn.com/click?url=https://amazon.com/...
     ```
     OR
     ```
     https://www.amazon.com/...?tag=sovrn-xxxxx
     ```
   - **Not Working:** Will show original URL:
     ```
     https://www.amazon.com/s?k=solar+panel+kits
     ```

### Method 3: Sovrn Dashboard Check

1. **Add `amazon.com` to Sovrn**
2. **Check if Sovrn auto-converts:**
   - Look for "Auto-link" or "Automatic Link Conversion" feature
   - If available, enable it
   - If not available, domain-level tracking probably doesn't work

3. **Check for tracking code:**
   - Sovrn usually provides a JavaScript snippet
   - This snippet automatically converts links on page load
   - Without this script, automatic conversion won't work

### Method 4: Click Test (After Setup)

1. **Visit your live site**
2. **Click an Amazon link** (use a test product you can track)
3. **Check URL in browser address bar after click:**
   - Should redirect through Sovrn tracking first
   - URL will contain Sovrn tracking parameters
4. **Check Sovrn dashboard after 24-48 hours:**
   - Look for "Clicks" or "Traffic" data
   - If you see clicks tracked, it's working!

---

## ✅ SIGNS IT'S WORKING:

- Amazon links on your site have Sovrn tracking URLs when inspected
- Sovrn dashboard shows "clicks" or traffic after testing
- Browser shows redirect through Sovrn domain when clicking links
- URLs contain tracking parameters (e.g., `?tag=`, `?ref=`, `aff_id=`)

## ❌ SIGNS IT'S NOT WORKING:

- Links still show original Amazon URLs (no conversion)
- No tracking script installed/required by Sovrn
- Sovrn requires individual links instead of domain-level
- No clicks appear in Sovrn dashboard after testing

---

## 🔧 IF SIMPLE METHOD DOESN'T WORK:

If domain-level tracking doesn't work, you'll need to:

1. **Use the detailed link list** from `SOVRN_LINKS_SIMPLE.md`
2. **Create individual affiliate links** for each URL in Sovrn
3. **Replace links manually** in your code

---

## 📝 QUICK TEST CHECKLIST:

- [ ] Added `amazon.com` to Sovrn
- [ ] Installed Sovrn tracking script (if required)
- [ ] Checked one Amazon link on live site - URL converted?
- [ ] Clicked test link - redirected through Sovrn?
- [ ] Checked Sovrn dashboard - clicks showing?

**If all checked = Simple method works!** ✅
**If links not converting = Use detailed method** 📋

