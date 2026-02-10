# Soft Robotics Design Lab Website

A modern, professional website for the Soft Robotics Design Lab built with GitHub Pages.

## 🚀 Quick Setup Guide

### Step 1: Create a GitHub Repository
1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `SoftRoboticsDesignLab` (or any name you prefer)
3. Make it public
4. Initialize with a README (optional)

### Step 2: Upload Your Website
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/YOUR-USERNAME/SoftRoboticsDesignLab.git
   cd SoftRoboticsDesignLab
   ```

2. Copy the `index.html` file into the repository folder

3. Commit and push:
   ```bash
   git add index.html
   git commit -m "Add lab website"
   git push origin main
   ```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings**
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select **main** branch
5. Click **Save**
6. Your site will be published at: `https://YOUR-USERNAME.github.io/SoftRoboticsDesignLab/`

## ✏️ Customization Guide

### Update Lab Information
Edit the `index.html` file to customize:

1. **Hero Section** (lines 175-182):
   - Update lab name and description
   - Modify tagline

2. **Research Areas** (lines 188-227):
   - Add/remove research cards
   - Update descriptions and icons

3. **Team Section** (lines 231-251):
   - Replace placeholder names with actual team members
   - Add photos by replacing the `.member-photo` divs with `<img>` tags

4. **Publications** (lines 255-274):
   - Add your actual publications
   - Update authors, titles, and venues

5. **Contact Information** (lines 280-307):
   - Update location details
   - Add real email address
   - Update social media links

### Add Team Photos
Replace the placeholder circles with actual photos:

```html
<!-- Replace this: -->
<div class="member-photo">PI</div>

<!-- With this: -->
<img src="images/team/dr-name.jpg" alt="Dr. Name" style="width: 180px; height: 180px; border-radius: 50%; object-fit: cover;">
```

### Change Colors
The website uses UTEP's official colors. Modify the CSS variables if needed (lines 10-17):

```css
:root {
    --primary: #041E42;      /* UTEP Navy Blue */
    --secondary: #FF8200;    /* UTEP Orange */
    --accent: #FF8200;       /* UTEP Orange accent */
    --dark: #041E42;         /* Dark navy text */
    --light: #F8F9FA;        /* Background */
    --gray: #6C757D;         /* Muted text */
}
```

### Add Additional Sections
You can add new sections following this template:

```html
<section id="new-section">
    <div class="container">
        <h2>Section Title</h2>
        <p>Your content here...</p>
    </div>
</section>
```

Don't forget to add a navigation link:
```html
<li><a href="#new-section">Section Name</a></li>
```

## 📁 Recommended Folder Structure

```
SoftRoboticsDesignLab/
├── index.html
├── README.md
├── images/
│   ├── team/
│   │   ├── pi.jpg
│   │   ├── member1.jpg
│   │   └── member2.jpg
│   ├── research/
│   │   └── project-images.jpg
│   └── logo.png
└── publications/
    └── papers.pdf (optional)
```

## 🎨 Design Features

- **Responsive Design**: Works on all devices (desktop, tablet, mobile)
- **Smooth Animations**: Scroll-triggered animations and hover effects
- **Modern Typography**: Uses Spectral (serif) and IBM Plex Mono (monospace)
- **UTEP Colors**: Official University of Texas at El Paso orange (#FF8200) and navy blue (#041E42)
- **Fixed Navigation**: Easy access to all sections
- **Clean Layout**: Focus on readability and content hierarchy

## 🔧 Advanced Customization

### Adding Google Analytics
Add before the closing `</head>` tag:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### Custom Domain
1. Purchase a domain (e.g., `softroboticslab.com`)
2. In repository Settings > Pages, add your custom domain
3. Update DNS settings with your domain provider

## 📝 License

Feel free to use and modify this template for your research lab website.

## 🆘 Support

For questions about GitHub Pages, visit the [official documentation](https://docs.github.com/en/pages).
