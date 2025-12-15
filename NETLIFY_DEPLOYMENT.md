# Netlify Deployment Guide

This guide will help you deploy your portfolio website to Netlify.

## Quick Start (3 Steps)

### 1. Sign Up for Netlify
- Go to [app.netlify.com](https://app.netlify.com)
- Sign up with GitHub, GitLab, Bitbucket, or email (GitHub recommended)

### 2. Deploy Your Site

**Option A: Drag & Drop (Fastest)**
1. Click "Add new site" → "Deploy manually"
2. Drag and drop your entire project folder onto the deployment area
3. Wait 30 seconds for deployment
4. Your site is live! 🎉

**Option B: Git Integration (Recommended)**
1. Push your code to GitHub/GitLab/Bitbucket
2. In Netlify, click "Add new site" → "Import an existing project"
3. Connect your Git repository
4. Netlify will auto-detect settings (no build command needed)
5. Click "Deploy site"
6. Future updates: Just push to your repo and Netlify auto-deploys!

### 3. Configure Contact Form

After deployment, set up email notifications:
1. Go to your site dashboard in Netlify
2. Navigate to **Forms** in the left sidebar
3. You should see your "contact" form listed
4. Click on the form → **Settings & spam**
5. Under **Email notifications**, click "Add notification"
6. Add your email address
7. Save

Now you'll receive email notifications when someone submits the contact form!

## Custom Domain

**For detailed instructions, see [`DOMAIN_SETUP.md`](DOMAIN_SETUP.md)**

Quick setup:

1. **In Netlify:**
   - Go to Site settings → Domain management
   - Click "Add custom domain"
   - Enter your domain (e.g., `yourname.com`)

2. **Configure DNS at your registrar:**
   - Add DNS records (see `DOMAIN_SETUP.md` for Register.com specific steps)
   - Type: `A`, Name: `@`, Value: `75.2.60.5`
   - Type: `CNAME`, Name: `www`, Value: `your-site.netlify.app`
   - Wait for DNS propagation (24-48 hours, usually faster)

**For Register.com domains:** See the detailed guide in `DOMAIN_SETUP.md`

## Netlify Forms Features

Your contact form automatically:
- ✅ Captures all form submissions
- ✅ Provides spam protection (honeypot + Akismet)
- ✅ Supports file attachments (up to 8MB per file)
- ✅ Stores submissions in Netlify dashboard
- ✅ Sends email notifications (when configured)

**Free Tier Limits:**
- 100 form submissions per month
- File uploads: 8MB per file
- Perfect for a portfolio site!

## Environment Variables (If Needed Later)

If you add features requiring API keys:
1. Go to Site settings → Environment variables
2. Add your variables
3. Redeploy the site

## Preview Deploys

When using Git integration:
- Every pull request gets a preview URL
- Test changes before merging to main branch
- Preview URLs look like: `deploy-preview-123--your-site.netlify.app`

## Troubleshooting

**Form not working?**
- Make sure you deployed the updated `contact.html` with `data-netlify="true"`
- Check the Forms section in Netlify dashboard to see if submissions are coming through
- Verify email notifications are configured

**Site not updating?**
- Clear your browser cache
- Check Netlify deploy log for errors
- Ensure you pushed changes to your Git repository (if using Git integration)

**Need help?**
- [Netlify Documentation](https://docs.netlify.com/)
- [Netlify Community](https://answers.netlify.com/)

## Next Steps

1. ✅ Deploy your site
2. ✅ Configure email notifications for forms
3. ✅ Add your images (see `IMAGES_GUIDE.md`)
4. ✅ Customize content (artist name, descriptions, etc.)
5. ✅ Set up custom domain (optional)

Your portfolio is ready to share with the world! 🌟

