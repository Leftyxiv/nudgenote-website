# 🚀 LAUNCH CHECKLIST

When NudgeNote is approved and ready to launch, search for `LAUNCH TODO` comments throughout the codebase and make these changes:

## 📋 Quick Search Commands
```bash
# Find all launch TODOs
grep -r "LAUNCH TODO" src/

# Find all disabled buttons
grep -r "btn--disabled" src/
```

## 🔄 Changes Needed

### 1. **Homepage** (`src/pages/index.astro`)
- [ ] Replace 4 disabled buttons with App Store links
- [ ] Update hero text: "Currently in development • Stay tuned!" → "Free to start • No credit card required"
- [ ] Update CTA text: "In development for iPhone" → "Available for iPhone"
- [ ] Remove `.btn--disabled` CSS rule

### 2. **Header** (`src/components/Header.astro`)
- [ ] Replace disabled "Coming Soon" button with "Download" link
- [ ] Remove `.nav__cta--disabled` CSS rules

### 3. **Footer** (`src/components/Footer.astro`)
- [ ] Replace "Coming Soon" span with "Download" link
- [ ] Remove `.footer__disabled` CSS rule

### 4. **App Store URL**
Replace all instances of `YOUR_APP_ID` with actual App Store ID:
```
https://apps.apple.com/app/YOUR_APP_ID
```

## 🎯 Final Steps
1. Test all download links work correctly
2. Verify favicon appears in browser tabs
3. Test social media sharing shows logo
4. Remove this checklist file
5. Celebrate! 🎉

---
*This file can be deleted after launch* 