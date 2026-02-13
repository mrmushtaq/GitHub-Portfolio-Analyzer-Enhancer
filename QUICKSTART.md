# 🚀 Quick Start Guide

## Get Running in 3 Steps

### Step 1: Open the Tool
**Option A - Direct Open (Easiest)**
1. Download/clone this repository
2. Double-click `index.html`
3. That's it! The tool opens in your browser

**Option B - GitHub Pages (For Sharing)**
1. Fork this repository on GitHub
2. Go to Settings → Pages
3. Select `main` branch → Save
4. Visit `https://yourusername.github.io/github-analyzer`

**Option C - Deploy to Vercel/Netlify (Professional)**
1. Sign up for free account
2. Import this repository
3. Click deploy
4. Get a custom URL to share

### Step 2: Analyze a Profile
1. Enter any GitHub username (try `torvalds` or `gaearon`)
2. Click "Analyze Profile"
3. Wait 10-20 seconds for results

### Step 3: Review & Improve
1. Check your overall score
2. Review the 6 metrics
3. Read prioritized recommendations
4. Take action on HIGH priority items first!

---

## 📱 Test It Right Now

**Try these profiles:**
- `torvalds` - Linux creator (strong profile)
- `gaearon` - React core team (excellent docs)
- `yours` - Your own username!

---

## 🎯 What You Get

### Portfolio Score (0-100)
- **80-100**: Excellent! Recruiter-ready ⭐
- **60-79**: Good foundation, room to improve 👍
- **0-59**: Needs significant work ⚠️

### 6 Key Metrics
1. **Documentation Quality** - READMEs, descriptions, demos
2. **Code Quality** - Structure, languages, best practices
3. **Activity Consistency** - Commit frequency, recent work
4. **Repository Organization** - Naming, licenses, pinning
5. **Project Impact** - Stars, forks, community engagement
6. **Technical Depth** - Skill breadth and complexity

### Actionable Recommendations
- 🔴 **HIGH** priority - Fix these first!
- 🟡 **MEDIUM** priority - Important improvements
- 🔵 **LOW** priority - Nice to have enhancements

---

## 💻 No Installation Required!

This tool:
- ✅ Runs entirely in your browser
- ✅ No sign-up or registration
- ✅ No data stored or collected
- ✅ Works offline after first load
- ✅ No npm install, no dependencies
- ✅ Works on all devices

---

## 🛠️ For Developers

### Customize the Scoring
Edit weights in `index.html` around line 500:
```javascript
const overallScore = Math.round(
    (documentationScore * 0.25) +  // Change these!
    (codeQualityScore * 0.20) +
    // ...
);
```

### Add New Metrics
1. Create calculation function
2. Add to analysis object
3. Update display grid
4. Add description text

### Modify UI Colors
Search for `#667eea` and `#764ba2` to change the gradient theme

---

## 📊 Score Breakdown

Each metric is scored 0-100 based on:

**Documentation (25% weight)**
- Descriptions present (40%)
- Demo links available (30%)
- Topic tags used (30%)

**Code Quality (20% weight)**
- Language diversity (40%)
- Project substance (30%)
- Collaboration features (30%)

**Activity (15% weight)**
- Push frequency (40%)
- Recency (30%)
- Updated repos (30%)

**Organization (15% weight)**
- Engagement (40%)
- Licenses (30%)
- Naming (30%)

**Impact (15% weight)**
- Stars (40%)
- Forks (40%)
- Watchers (20%)

**Technical Depth (10% weight)**
- Languages (60%)
- Complexity (40%)

---

## 🎬 Making Your Demo Video

### What to Record (2-3 minutes)
1. **Introduction** (15 sec)
   - "Hi, this is GitHub Portfolio Analyzer"
   - Quick problem statement

2. **Demo** (90 sec)
   - Enter a username
   - Show loading
   - Highlight score
   - Show metrics
   - Read 2-3 recommendations

3. **Key Features** (30 sec)
   - Real-time analysis
   - Actionable insights
   - No setup required

4. **Conclusion** (15 sec)
   - Benefits for students
   - How to access

### Tools to Use
- **Free:** OBS Studio, QuickTime, Windows Game Bar
- **Paid:** Camtasia, ScreenFlow, Loom

### Tips
- ✅ Use a real GitHub profile
- ✅ Keep it under 3 minutes
- ✅ Show the actual tool working
- ✅ Highlight actionable recommendations
- ✅ Mention it takes <2 minutes to analyze

---

## 🚨 Troubleshooting

**"GitHub user not found"**
- Check username spelling
- Try without the @ symbol
- Ensure profile is public

**"API rate limit exceeded"**
- GitHub limits to 60 requests/hour without auth
- Wait an hour or use a different network
- For production, add GitHub token

**Blank page after clicking analyze**
- Check browser console (F12)
- Ensure internet connection
- Try a different browser

**Scores seem wrong**
- Algorithm weights certain factors
- Check individual metrics for details
- Remember it's objective, not perfect

---

## 📞 Support

- **Issues:** Open a GitHub issue
- **Questions:** info@unsaidtalks.com
- **WhatsApp:** +91-7303573374

---

## ✅ Submission Checklist

Before submitting to the hackathon:

- [ ] Test with at least 5 different profiles
- [ ] Record demo video (2-3 minutes)
- [ ] Add demo video link to README
- [ ] Test on mobile device
- [ ] Verify all links work
- [ ] Check README formatting
- [ ] Ensure repository is PUBLIC
- [ ] Test deployed version (optional but recommended)
- [ ] Add screenshots to README (optional)
- [ ] Write clear commit messages

---

## 🎓 Learning Resources

Want to improve your GitHub profile? Check out:
- [GitHub Docs - Profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile)
- [makeareadme.com](https://www.makeareadme.com/)
- [Choose a License](https://choosealicense.com/)
- [Shields.io - Badges](https://shields.io/)

---

**Made with ❤️ for the UnsaidTalks Hackathon**

*Last Updated: February 13, 2026*
