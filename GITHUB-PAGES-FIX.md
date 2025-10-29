# 🔍 GITHUB PAGES TROUBLESHOOTING GUIDE

## **Problem: 404 Error on Blog Pages**

### **Most Common Causes:**

1. **Files Not Uploaded to GitHub**
   - Check your GitHub repo in the browser
   - Verify the `blog/` folder exists in your repo
   - Make sure all files are committed and pushed

2. **Wrong Branch/Directory**
   - GitHub Pages might be serving from `/docs` folder
   - Or serving from `gh-pages` branch instead of `main`
   - Check: Settings → Pages → Source

3. **GitHub Pages Not Rebuilt**
   - Wait 2-5 minutes after upload
   - Check: Actions tab → Latest workflow run

4. **Case Sensitivity**
   - GitHub Pages is case-sensitive
   - Make sure `blog/` folder is lowercase

## **✅ VERIFICATION CHECKLIST:**

### **Step 1: Check GitHub Repo Structure**
Your repo should have this structure:
```
your-repo-name/
├── index.html
├── blog/
│   ├── index.html
│   ├── test.html
│   ├── driving-co2-per-mile.html
│   ├── chicken-vs-beef-footprint.html
│   └── offset-carbon-cheap.html
├── assets/
│   └── (image files)
└── sitemap.xml
```

### **Step 2: Verify GitHub Pages Settings**
1. Go to your repo → **Settings** → **Pages**
2. **Source:** Should be set to your branch (usually `main` or `master`)
3. **Branch:** Should be `/ (root)`
4. **Custom domain:** Should show `carbonchecks.com`

### **Step 3: Check GitHub Actions**
1. Go to **Actions** tab in your repo
2. Look for any failed builds
3. If there are errors, fix them

### **Step 4: Test Direct URLs**
Try these URLs in order:
1. `https://carbonchecks.com/blog/` (should load blog/index.html)
2. `https://carbonchecks.com/blog/index.html` (explicit path)
3. `https://carbonchecks.com/blog/test.html` (test file)

## **🚀 QUICK FIXES:**

### **Fix 1: Force GitHub Pages Rebuild**
1. Make a small change to any file (add a space)
2. Commit and push
3. Wait 2-3 minutes
4. Try again

### **Fix 2: Check Branch Deployment**
If your files are in a different branch:
1. Go to Settings → Pages
2. Change source branch to where your files are
3. Save and wait

### **Fix 3: Verify File Upload**
1. Go to your GitHub repo in browser
2. Navigate to `blog/` folder
3. Check if `index.html` exists there
4. If not, upload it!

## **📝 NEXT STEPS:**

1. **Upload all files** from `CARBON-UPLOAD` folder to your GitHub repo
2. **Make sure** they're in the root directory (not in a subfolder)
3. **Wait 3-5 minutes** for GitHub Pages to rebuild
4. **Test** the blog link again

## **🎯 Current Status:**

- ✅ Files exist locally in `CARBON-UPLOAD/blog/`
- ✅ Paths are fixed (using relative paths)
- ⏳ Waiting for GitHub Pages deployment
- ❓ Need to verify files are uploaded to GitHub

---
**If you've already uploaded, wait 3-5 minutes and try again!** 🚀
