# Portfolio Madre

A simple, elegant artist portfolio website with a monochromatic design.

## Features

- Large banner section with artist name and subtitle
- Horizontal scrolling gallery of artwork
- About Me page with artist information
- Contact form with file attachment support
- Clean, monochromatic design
- Responsive layout

## Getting Started

### Option 1: Using npm/http-server (Recommended)

1. Install dependencies (if you have Node.js installed):
   ```bash
   npm install
   ```

2. Start the local server:
   ```bash
   npm start
   ```

   This will automatically open your browser to `http://localhost:8080`

### Option 2: Using Python

If you have Python installed:

```bash
# Python 3
python -m http.server 8080

# Python 2
python -m SimpleHTTPServer 8080
```

Then open your browser to `http://localhost:8080`

### Option 3: Direct File Opening

Simply open `index.html` directly in your web browser. Note that some features may be limited when opening files directly.

## Contact Form Setup

The contact form uses **Netlify Forms**, which is automatically enabled when you deploy to Netlify. No additional setup required!

**Features:**
- ✅ Free tier: 100 submissions per month
- ✅ Automatic spam protection
- ✅ File attachments supported (up to 8MB per file)
- ✅ Email notifications (configure in Netlify dashboard)
- ✅ Form submissions stored in Netlify dashboard

**To configure email notifications:**
1. Deploy your site to Netlify
2. Go to your site dashboard → Forms
3. Click on "Settings" for the contact form
4. Add your email address to receive notifications

**Note:** The form works automatically when deployed to Netlify. No API keys or external services needed!

## Adding Images

See `IMAGES_GUIDE.md` for detailed instructions on how to add:
- Banner background image
- Gallery artwork images
- Artist photo on the About page

Quick guide:
1. Create an `images` folder in your project root
2. Organize images into subfolders: `banner/`, `gallery/`, `about/`
3. Replace placeholder divs with `<img>` tags (examples are commented in the HTML files)
4. Update image paths in the HTML/CSS files

## Customization

- Edit `index.html` to change the artist name, subtitle, and gallery items
- Edit `about.html` to update artist information and description
- Edit `contact.html` to customize the contact form
- Edit `styles.css` to customize colors, fonts, and layout

## Deployment to Netlify

This site is configured for easy deployment to Netlify. You have two options:

### Option 1: Deploy via Netlify Dashboard (Easiest)

1. Go to [app.netlify.com](https://app.netlify.com) and sign up/login
2. Click "Add new site" → "Deploy manually"
3. Drag and drop your project folder onto the deployment area
4. Your site will be live in seconds!

### Option 2: Deploy via Git (Recommended for updates)

1. Push your code to GitHub, GitLab, or Bitbucket
2. Go to [app.netlify.com](https://app.netlify.com) and sign up/login
3. Click "Add new site" → "Import an existing project"
4. Connect your Git repository
5. Netlify will auto-detect settings (no build command needed)
6. Click "Deploy site"
7. Every time you push to your repo, Netlify will automatically deploy updates

### Custom Domain

After deployment, you can add a custom domain:
1. Go to Site settings → Domain management
2. Click "Add custom domain"
3. Follow the instructions to configure DNS

### Form Setup

The contact form automatically works when deployed to Netlify. To receive email notifications:
1. Go to Forms in your Netlify dashboard
2. Configure email notifications for form submissions

## Project Structure

```
Portfolio Madre/
├── index.html      # Main homepage
├── about.html      # About Me page
├── contact.html    # Contact form page (Netlify Forms)
├── styles.css      # Styling
├── netlify.toml    # Netlify configuration
├── package.json    # npm configuration
└── README.md       # This file
```
