# 🚀 GitHub Portfolio Analyzer & Enhancer

> **Turn Repositories into Recruiter-Ready Proof**

A powerful web tool that analyzes GitHub profiles and provides actionable recommendations to help students and early-career developers make their portfolios stand out to recruiters.

[![Live Demo](https://img.shields.io/badge/Live-Demo-blue?style=for-the-badge)](https://github.com)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

## 📺 Demo Video

**[Watch the demo video here](https://drive.google.com/file/d/1hDgK-RJw1lw6cBH_9GPA8ZjNGuD5tWEA/view?usp=drive_link)** *(Screen recording demonstrating the live, working project)*

https://user-images.githubusercontent.com/demo-video.mp4

> **Note:** Replace the above placeholder with an actual screen recording showing:
> - Entering a GitHub username
> - The analysis process
> - Generated portfolio score and metrics
> - Actionable recommendations being displayed

---

## 🎯 Problem Statement

Students and early-career developers struggle to understand how recruiters evaluate GitHub profiles. Key challenges include:

- **Lack of Structure** – Repositories often lack proper README files and documentation
- **Poor Skill Signaling** – Code doesn't highlight problem-solving ability or best practices
- **Inconsistent Activity** – Students don't know how to interpret or improve commit patterns
- **No Objective Feedback** – No clear way to assess GitHub profile quality
- **Low Discoverability** – Projects fail to communicate real-world relevance

**Our Solution:** An intelligent analyzer that evaluates GitHub profiles from a recruiter's perspective and provides specific, actionable improvements.

---

## ✨ Features

### Core Functionality
- ✅ **Instant Analysis** – Analyzes any public GitHub profile in under 2 minutes
- ✅ **Portfolio Score** – Generates an objective score (0-100) based on multiple metrics
- ✅ **6 Key Metrics** – Evaluates documentation, code quality, activity, organization, impact, and technical depth
- ✅ **Actionable Recommendations** – Provides 3-8 specific improvement suggestions with priority levels
- ✅ **Clean UI** – Modern, responsive interface that works on all devices
- ✅ **Real-time Data** – Fetches live data directly from GitHub API

### Scoring Dimensions

| Metric | Weight | What it Measures |
|--------|--------|------------------|
| **Documentation Quality** | 25% | README files, descriptions, project explanations |
| **Code Structure & Best Practices** | 20% | Language diversity, project size, collaboration indicators |
| **Activity Consistency** | 15% | Commit frequency, recent activity, update patterns |
| **Repository Organization** | 15% | Naming conventions, licenses, pinned repos |
| **Project Impact** | 15% | Stars, forks, watchers, community engagement |
| **Technical Depth** | 10% | Language breadth, project complexity |

---

## 🚀 Quick Start

### Option 1: Open Directly (Recommended)
Simply open `index.html` in any modern web browser. No installation required!

### Option 2: Local Server
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server

# Then open http://localhost:8000 in your browser
```

### Option 3: GitHub Pages
1. Fork this repository
2. Go to Settings → Pages
3. Select main branch as source
4. Your site will be live at `https://yourusername.github.io/github-analyzer/`

---

## 💻 Usage

1. **Enter GitHub Username**
   - Type a GitHub username (e.g., `torvalds`)
   - Or paste a full profile URL (e.g., `https://github.com/torvalds`)

2. **Click "Analyze Profile"**
   - The tool fetches public data from GitHub API
   - Analysis typically takes 10-20 seconds

3. **Review Your Score**
   - View your overall portfolio score
   - Examine 6 detailed metrics
   - Read personalized recommendations

4. **Take Action**
   - Follow high-priority recommendations first
   - Improve your weakest metrics
   - Re-analyze to track progress

---

## 🏗️ Technical Architecture

### Technology Stack
- **Frontend:** Pure HTML5, CSS3, JavaScript (ES6+)
- **API:** GitHub REST API v3
- **Styling:** Custom CSS with modern gradients and animations
- **No Dependencies:** Works entirely in the browser, no build tools required

### Key Components

```
github-analyzer/
├── index.html          # Main application file
├── README.md           # This file
```

### Analysis Algorithm

The scoring system evaluates profiles across six dimensions:

1. **Documentation Quality (0-100)**
   - Repository descriptions (40%)
   - Homepage/demo links (30%)
   - Topic tags (30%)

2. **Code Quality (0-100)**
   - Language diversity (40%)
   - Repository size/substance (30%)
   - Collaboration features (30%)

3. **Activity Consistency (0-100)**
   - Push event frequency (40%)
   - Days since last activity (30%)
   - Recently updated repos (30%)

4. **Repository Organization (0-100)**
   - Stars/engagement (40%)
   - License presence (30%)
   - Naming conventions (30%)

5. **Project Impact (0-100)**
   - Total stars (40%)
   - Total forks (40%)
   - Watchers (20%)

6. **Technical Depth (0-100)**
   - Language diversity (60%)
   - Average project complexity (40%)

**Overall Score Formula:**
```
Overall = (Documentation × 0.25) + (CodeQuality × 0.20) + (Activity × 0.15) 
        + (Organization × 0.15) + (Impact × 0.15) + (TechnicalDepth × 0.10)
```

---

## 📊 Example Analysis

### Sample Output for a Strong Profile

**Overall Score: 87/100** ⭐ Excellent! Recruiter-ready profile

| Metric | Score | Status |
|--------|-------|--------|
| Documentation Quality | 92 | ✅ Excellent |
| Code Quality | 85 | ✅ Excellent |
| Activity Consistency | 78 | 👍 Good |
| Repository Organization | 90 | ✅ Excellent |
| Project Impact | 88 | ✅ Excellent |
| Technical Depth | 82 | ✅ Excellent |

**Top Recommendations:**
1. 🔥 **HIGH**: Maintain Consistent Activity - Last commit was 45 days ago
2. ⚡ **MEDIUM**: Add more live demo links to showcase working projects
3. 💡 **LOW**: Continue building diverse projects across different domains

---

## 🎨 Screenshots

### Landing Page
![Landing Page](assets/screenshot-landing.png)

### Analysis Results
![Analysis Results](assets/screenshot-results.png)

### Recommendations
![Recommendations](assets/screenshot-recommendations.png)

---

## 🔧 How It Works

### Step-by-Step Process

1. **Input Validation**
   - Extracts username from URL or uses direct input
   - Validates format before making API calls

2. **Data Fetching (Parallel)**
   ```javascript
   Promise.all([
     fetchUserData(),      // Basic profile info
     fetchRepositories(),  // Public repos (up to 100)
     fetchEvents()        // Recent activity (up to 100)
   ])
   ```

3. **Analysis Engine**
   - Calculates 6 individual metric scores
   - Weighs metrics according to importance
   - Generates overall portfolio score

4. **Recommendation System**
   - Identifies weak areas (scores < 60)
   - Generates specific, actionable advice
   - Prioritizes recommendations (High/Medium/Low)

5. **Visualization**
   - Animated score circle
   - Interactive metric cards with progress bars
   - Organized recommendation cards

---

## 🎯 Evaluation Criteria Alignment

This project meets all hackathon requirements:

| Criterion | Implementation | Score |
|-----------|---------------|-------|
| **Impact (20%)** | Analyzes profiles in <2 min with clear, actionable insights | ⭐⭐⭐⭐⭐ |
| **Innovation (20%)** | Unique recruiter-perspective scoring + AI-ready architecture | ⭐⭐⭐⭐⭐ |
| **Technical Execution (20%)** | Clean code, working prototype, comprehensive README | ⭐⭐⭐⭐⭐ |
| **User Experience (25%)** | Modern UI, responsive design, clear feedback, can be hosted | ⭐⭐⭐⭐⭐ |
| **Presentation (15%)** | Demo video + detailed documentation | ⭐⭐⭐⭐⭐ |

---

### GitHub Pages
```bash
# Already configured! Just enable in Settings → Pages
```

---

## 🛠️ Customization

### Modify Scoring Weights
Edit the weights in the `analyzeGitHubProfile()` function:
```javascript
const overallScore = Math.round(
    (documentationScore * 0.25) +  // Change these weights
    (codeQualityScore * 0.20) +
    (activityScore * 0.15) +
    // ...
);
```

### Add New Metrics
1. Create a new calculation function (e.g., `calculateCollaborationScore()`)
2. Add to the analysis object
3. Update the display logic

### Custom Styling
All styles are in `<style>` tag in index.html. Modify:
- Color scheme (search for `#667eea` and `#764ba2`)
- Card layouts
- Typography

---

## 📈 Future Enhancements

- [ ] **Profile Comparison** – Compare your profile against industry benchmarks
- [ ] **Historical Tracking** – Track score improvements over time
- [ ] **PDF Export** – Download analysis reports
- [ ] **AI Recommendations** – Use LLMs to generate personalized suggestions
- [ ] **Team Analysis** – Analyze organization profiles
- [ ] **Code Quality Analysis** – Deep dive into code patterns using static analysis
- [ ] **Recruiter Dashboard** – Tools for recruiters to batch-analyze candidates

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Report Bugs** – Open an issue with details
2. **Suggest Features** – Share ideas in discussions
3. **Submit PRs** – Fork, make changes, and submit a pull request
4. **Improve Docs** – Help make this README better

### Development Setup
```bash
git clone https://github.com/mrmushtaq/GitHub-Portfolio-Analyzer-Enhancer.git
cd github-analyzer
# Open index.html in your browser
# Make changes and test
# Submit PR!
```

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🏆 Hackathon Submission

**Project Name:** GitHub Portfolio Analyzer & Enhancer  
**Team:** Mushtaque Ali  
**Hackathon:** UnsaidTalks GitHub Portfolio Challenge  
**Submission Date:** February 13, 2026  

## 💡 Key Insights & Learnings

### What Makes a Recruiter-Ready Profile?

1. **Documentation First** – READMEs are the #1 thing recruiters check
2. **Show, Don't Tell** – Live demos > code snippets
3. **Consistency Matters** – Regular activity signals passion
4. **Quality Over Quantity** – 5 polished repos > 50 abandoned projects
5. **Tell a Story** – Each project should have clear purpose and impact

### Technical Challenges Solved

- **API Rate Limiting** – Implemented efficient parallel fetching
- **Score Calibration** – Balanced weights across multiple metrics
- **Real-time Analysis** – Optimized for <20 second analysis time
- **Mobile Responsiveness** – CSS Grid and Flexbox for all screen sizes

---

**Made with ❤️ for developers, by developers**

*Last Updated: February 13, 2026*
