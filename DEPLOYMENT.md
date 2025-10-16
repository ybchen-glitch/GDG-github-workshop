# 🚀 GitHub Pages Deployment Guide

## Quick Setup (5 minutes)

### Step 1: Create GitHub Repository
1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Name your repository (e.g., `my-portfolio`, `personal-website`)
4. Make it **Public** (required for free GitHub Pages)
5. Don't initialize with README (we already have files)
6. Click "Create repository"

### Step 2: Upload Your Files
You can upload files in two ways:

#### Option A: Web Interface (Easiest)
1. On your new repository page, click "uploading an existing file"
2. Drag and drop all files from `Website_demo_v2` folder:
   - `index.html`
   - `README.md`
   - `_config.yml`
   - `.gitignore`
3. Write a commit message: "Initial portfolio upload"
4. Click "Commit changes"

#### Option B: Git Commands (If you have Git installed)
```bash
# Navigate to your Website_demo_v2 folder
cd path/to/Website_demo_v2

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio upload"

# Add your GitHub repository as remote (replace with your URL)
git remote add origin https://github.com/yourusername/your-repository-name.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

### Step 4: Access Your Website
- GitHub will provide a URL like: `https://yourusername.github.io/repository-name`
- It may take 5-10 minutes for the site to be live
- You'll see a green checkmark when deployment is complete

## 📝 Before You Deploy - Customize Your Content!

### Essential Updates in `index.html`:
1. **Replace "Name"** with your actual name
2. **Update "Subtitle"** with your role/title
3. **Change profile image** - replace the image URL or upload your own photo
4. **Add your contact info**:
   - Email address
   - Phone number
   - LinkedIn profile URL
5. **Fill in Education section**:
   - School name
   - Degree and major
6. **Add Work Experience**:
   - Job titles
   - Company names
   - Job descriptions
7. **Showcase Projects**:
   - Project names
   - Descriptions
   - Links to live projects or GitHub repos

### Optional: Update `_config.yml`:
- Change `title`, `description`, and `author`
- Add your email and social media handles

## 🔧 Making Updates

After your site is live, you can update it by:

1. **Web Interface**: Edit files directly on GitHub
2. **Local Development**: 
   - Make changes locally
   - Commit and push to update the live site

## 🎨 Customization Ideas

### Add Your Own Photo
1. Upload your photo to the repository
2. Update the image source in `index.html`:
   ```html
   <img src="your-photo.jpg" class="img-fluid" alt="Your Name">
   ```

### Change Colors
Use Bootstrap utility classes:
```html
<h1 class="fw-bold text-primary">Your Name</h1>
<div class="container bg-light p-4">Content</div>
```

### Add More Sections
```html
<div class="container mt-5">
    <h2 class="fw-bold">Skills</h2>
    <p>List your technical skills here</p>
</div>
```

## 🆘 Troubleshooting

### Site Not Loading?
- Wait 10-15 minutes after enabling Pages
- Check that repository is public
- Verify files are in the root directory (not in a subfolder)

### Changes Not Showing?
- Wait a few minutes for GitHub to rebuild
- Hard refresh your browser (Ctrl+F5 or Cmd+Shift+R)
- Check the Actions tab for build status

### Need Help?
- Check [GitHub Pages documentation](https://docs.github.com/en/pages)
- Ensure your repository is public
- Verify all files are properly uploaded

## ✅ Deployment Checklist

- [ ] Repository created and set to public
- [ ] All files uploaded (`index.html`, `README.md`, `_config.yml`, `.gitignore`)
- [ ] Personal information updated in `index.html`
- [ ] GitHub Pages enabled in repository settings
- [ ] Website URL working (may take 5-10 minutes)
- [ ] Content reviewed and looks good on mobile and desktop

**Your portfolio website will be live at**: `https://yourusername.github.io/repository-name`

🎉 **Congratulations! Your portfolio is now live on the internet!**