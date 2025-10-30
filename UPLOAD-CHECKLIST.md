# 🚀 UPLOAD CHECKLIST - CarbonChecks Blog

## **Files to Upload to GitHub Pages:**

### **1. Root Directory Files:**
- ✅ `index.html` (updated with blog link)
- ✅ `sitemap.xml` (updated with blog URLs)
- ✅ `robots.txt` (updated)

### **2. Blog Directory:**
- ✅ `blog/index.html` (blog homepage)
- ✅ `blog/driving-co2-per-mile.html`
- ✅ `blog/chicken-vs-beef-footprint.html`
- ✅ `blog/offset-carbon-cheap.html`
- ✅ `blog/test.html` (test file - can be deleted after testing)

### **3. Assets Directory:**
- ✅ `assets/driving-co2-per-mile.jpg`
- ✅ `assets/driving-co2-per-mile.webp`
- ✅ `assets/chicken-vs-beef-footprint.jpg`
- ✅ `assets/chicken-vs-beef-footprint.webp`
- ✅ `assets/offset-carbon-cheap.jpg`
- ✅ `assets/offset-carbon-cheap.webp`

## **🔧 What I Fixed:**

1. **Path Issues:** Changed all `/blog/` absolute paths to relative paths
2. **Navigation:** Fixed blog links in all pages to use `index.html`
3. **Breadcrumbs:** Updated breadcrumb navigation
4. **Test File:** Added `blog/test.html` for testing

## **📋 Testing Steps:**

### **After Upload:**
1. **Test the blog link:** `https://carbonchecks.com/blog/`
2. **Test individual posts:**
   - `https://carbonchecks.com/blog/driving-co2-per-mile.html`
   - `https://carbonchecks.com/blog/chicken-vs-beef-footprint.html`
   - `https://carbonchecks.com/blog/offset-carbon-cheap.html`
3. **Test the test file:** `https://carbonchecks.com/blog/test.html`

### **If Still Getting 404:**
1. **Wait 2-3 minutes** for GitHub Pages to rebuild
2. **Check GitHub Actions** for build errors
3. **Verify file structure** in your GitHub repo
4. **Try accessing:** `https://carbonchecks.com/blog/index.html` directly

## **🎯 Expected Results:**

- ✅ Blog link in header should work
- ✅ Blog index page should load with 3 articles
- ✅ Individual blog posts should load
- ✅ All internal links should work
- ✅ Images should display (even if placeholders)

## **🚨 Common Issues:**

1. **GitHub Pages needs time to rebuild** (2-5 minutes)
2. **Case sensitivity** - make sure filenames match exactly
3. **File permissions** - ensure files are in the repo root
4. **Cache issues** - try hard refresh (Ctrl+F5)

---

**Ready to upload!** All files are fixed and ready to go. 🚀

