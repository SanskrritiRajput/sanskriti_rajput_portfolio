# 🌟 Sanskriti Rajput - AI/ML Portfolio

A stunning dark mode portfolio showcasing AI/ML projects, achievements, and expertise.

## ✨ Features

- 🎨 **Dark Mode Design** - Professional navy/teal theme with yellow accents
- 🖼️ **Hero Section** - Large profile image with animated floating badges
- 📱 **Fully Responsive** - Works perfectly on mobile, tablet, and desktop
- ⚡ **Smooth Animations** - Typing effects, scroll animations, and interactive elements
- 📊 **Project Showcase** - Multiple images/videos per project with detailed descriptions
- 🏆 **Achievements Section** - Hackathon wins, certifications, and leadership roles
- 💬 **Contact Form** - Direct email integration with visible contact information
- 🎯 **Easy to Edit** - Well-commented code with clear edit sections

## 🎯 Design Philosophy

This portfolio stands out from generic templates by featuring:
- **Unique color scheme** - Teal/Navy gradient with vibrant yellow accents
- **Dynamic hero section** - Large photo with personality-driven copy
- **Rich project presentations** - Multiple screenshots and videos
- **Achievement-focused** - Highlighting competitive wins and certifications
- **Professional yet energetic** - Balancing technical depth with personality

## 📁 File Structure

```
portfolio/
├── index.html                      # Main HTML structure
├── styles.css                      # All styling (dark mode theme)
├── script.js                       # Animations and interactions
├── pretty_me.jpeg                  # Your profile photo
├── ops1.png, ops2.png, ops3.png   # Online Proctoring System screenshots
├── Screenshot_2025-05-23_084204.png # Brain Tumor Detection image
├── HVD_PORTFOLIO.mp4              # Hand Gesture demo video
├── MGD1.png, MGD2.png, MGD3.png   # Music Genre Detector screenshots
└── README.md                       # This file
```

## 🚀 Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click **"New Repository"** (green button)
3. Name it: `portfolio` or `Sanskriti-s-portfolio`
4. Make it **Public**
5. **DO NOT** initialize with README
6. Click **"Create repository"**

### Step 2: Upload Files

**Option A - Via GitHub Web Interface (Easiest):**

1. In your new repository, click **"uploading an existing file"**
2. Drag and drop ALL files from this folder:
   - index.html
   - styles.css
   - script.js
   - pretty_me.jpeg
   - All project images (ops1-3.png, MGD1-3.png, etc.)
   - HVD_PORTFOLIO.mp4
3. Add commit message: "Initial portfolio upload"
4. Click **"Commit changes"**

**Option B - Via Git Command Line:**

```bash
cd path/to/portfolio/folder
git init
git add .
git commit -m "Initial portfolio upload"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Click **"Pages"** in left sidebar
3. Under **"Source"**, select **"main"** branch
4. Click **"Save"**
5. Wait 2-3 minutes for deployment

### Step 4: Access Your Live Site

Your portfolio will be live at:
```
https://YOUR_USERNAME.github.io/portfolio/
```

Example: `https://sanskrritirajput.github.io/Sanskriti-s-portfolio/`

## ✏️ How to Edit Your Portfolio

### 🎨 **Change Colors**

Open `styles.css` and edit the CSS variables at the top:

```css
/* Find this section at line 1 */
:root {
    --color-primary: #14F1D9;      /* Bright Teal - CHANGE THIS! */
    --color-secondary: #FFB800;     /* Yellow - CHANGE THIS! */
    --bg-primary: #0A0E27;         /* Dark background - CHANGE THIS! */
}
```

### 📝 **Update Your Information**

Open `index.html` and search for these sections:

**Hero Text (Line ~50):**
```html
<div class="hero-greeting">Hey there! 👋</div>
<h1 class="hero-title">
    I'm <span class="gradient-text">Sanskriti Rajput</span>
</h1>
```

**About Me (Line ~150):**
```html
<p class="lead-text">
    I'm a Computer Science student... <!-- EDIT THIS -->
</p>
```

**Contact Info (Line ~600):**
```html
<a href="mailto:YOUR_EMAIL@gmail.com">
<a href="tel:+91YOUR_NUMBER">
```

### 🖼️ **Change Your Photo**

1. **Replace the image file:**
   - Upload your new photo to the repository
   - Name it `pretty_me.jpeg` (or update the HTML)

2. **Or update the HTML:**
   ```html
   <!-- Line ~65 in index.html -->
   <img src="YOUR_NEW_IMAGE.jpg" alt="Sanskriti Rajput">
   ```

### 🔗 **Add Project Links**

Open `index.html` and find the project sections:

```html
<!-- Find sections like this around line ~400 -->
<a href="#" class="project-link" data-project="proctoring">
    <i class="fab fa-github"></i> View Code
</a>
```

**Replace `#` with your actual links:**
```html
<a href="https://github.com/yourname/project-repo" class="project-link">
    <i class="fab fa-github"></i> View Code
</a>
<a href="https://your-demo-link.com" class="project-link">
    <i class="fas fa-external-link-alt"></i> Live Demo
</a>
```

### ➕ **Add New Projects**

Copy an existing project card in `index.html` and modify:

```html
<!-- Copy from line ~350 to ~450 (one complete project-card) -->
<div class="project-card">
    <div class="project-number">05</div> <!-- Change number -->
    <div class="project-content">
        <h3 class="project-title">Your New Project</h3>
        <p class="project-tech">Python • TensorFlow • etc</p>
        <p class="project-description">
            Your project description here...
        </p>
        <!-- Add your project images -->
        <div class="project-gallery">
            <img src="your-project-img.png" alt="Project">
        </div>
    </div>
</div>
```

### 📧 **Update Contact Links**

The contact form opens the user's email client. To change where it sends:

Open `script.js` and find:
```javascript
// Line ~95
const mailtoLink = `mailto:YOUR_EMAIL@gmail.com?subject=...`;
```

### 🎭 **Change Typing Effect Text**

Open `script.js` and edit the texts array:

```javascript
// Line ~40
const texts = [
    'AI/ML Engineer & Innovation Builder',  // CHANGE THESE!
    'Deep Learning Enthusiast',
    'Hackathon Winner',
    'Problem Solver'
];
```

## 🎯 Common Customizations

### Add Google Analytics

Add before `</head>` in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

### Add Resume Download

1. Upload your resume PDF to the repository
2. Add a button in the hero section:

```html
<a href="Sanskriti_Rajput_Resume.pdf" download class="btn btn-secondary">
    <span>Download Resume</span>
    <i class="fas fa-download"></i>
</a>
```

### Add More Social Links

In the hero social section (~line 80):

```html
<div class="hero-social">
    <!-- Add new social links here -->
    <a href="https://twitter.com/yourhandle" target="_blank" class="social-link">
        <i class="fab fa-twitter"></i>
    </a>
</div>
```

## 🐛 Troubleshooting

**Portfolio not loading?**
- Check that all files are in the root directory
- Verify GitHub Pages is enabled in Settings
- Wait 2-3 minutes after enabling Pages

**Images not showing?**
- Ensure image filenames match exactly (case-sensitive!)
- Check that images are uploaded to the repository
- Verify image paths in HTML (`src="image.png"`)

**Styling looks broken?**
- Make sure `styles.css` is in the same folder as `index.html`
- Check browser console for errors (F12)
- Clear browser cache (Ctrl+F5)

**Video not playing?**
- Some browsers block autoplay - this is normal
- Video will play when scrolled into view
- Ensure video file is uploaded and path is correct

## 📱 Testing Your Portfolio

**Before Deploying:**
1. Open `index.html` in your browser locally
2. Check all links work
3. Test responsiveness (F12 → Device toolbar)
4. Verify all images load
5. Test on mobile device

**After Deploying:**
1. Visit your GitHub Pages URL
2. Test all navigation links
3. Try the contact form
4. Check on different devices

## 💡 Pro Tips

1. **Optimize Images:**
   - Compress images before uploading (use TinyPNG.com)
   - Keep images under 500KB for faster loading

2. **SEO Optimization:**
   - Update the `<title>` tag in HTML
   - Add meta descriptions
   - Use descriptive alt text for images

3. **Regular Updates:**
   - Add new projects as you build them
   - Update achievements and certifications
   - Keep contact information current

4. **Custom Domain (Optional):**
   - Buy a domain (e.g., from Namecheap)
   - Add it in GitHub Pages settings
   - Update DNS records at your domain provider

## 📞 Need Help?

If you run into issues:
1. Check the GitHub Pages deployment log
2. Validate HTML/CSS (W3C Validator)
3. Check browser console for errors
4. Compare with working version

## 🎉 You're All Set!

Your portfolio is now live and ready to impress recruiters! Remember to:
- ✅ Add your actual project links
- ✅ Update contact information
- ✅ Share the link on LinkedIn
- ✅ Include it on your resume
- ✅ Keep it updated with new projects

---

**Built with 💙 using Claude AI**

Good luck with your internship search! 🚀
