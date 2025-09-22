# Two Men and AI - Manufacturing Technology Consulting Website

A professional, responsive website for Two Men and AI, specializing in manufacturing technology consulting and AI integration services.

## 🚀 Quick Start

This is a static HTML website that's ready to deploy immediately. No build process required!

### Files Included
- `index.html` - Complete website with embedded CSS and JavaScript
- `netlify.toml` - Netlify deployment configuration
- `docs/update-guide.md` - Instructions for updating content
- `.gitignore` - Git ignore patterns

## 🌐 Deployment Options

### Option 1: Netlify (Recommended)

1. **Create Netlify Account**
   - Go to [netlify.com](https://netlify.com) and sign up
   - Connect your GitHub account (optional but recommended)

2. **Deploy via Drag & Drop**
   - Zip all project files (or use Git deployment)
   - Drag the folder to Netlify's deployment area
   - Your site will be live immediately with a random URL

3. **Deploy via Git (Recommended)**
   - Push this project to a GitHub repository
   - Connect the repository to Netlify
   - Automatic deployments on every commit

4. **Custom Domain Setup**
   - In Netlify dashboard, go to Site Settings > Domain Management
   - Add custom domain: 2men.ai
   - Follow DNS configuration instructions
   - SSL certificate will be automatically provisioned

### Option 2: Other Hosting Providers

The website works with any static hosting service:
- **Vercel**: Simply connect your GitHub repo
- **GitHub Pages**: Enable in repository settings
- **AWS S3**: Upload files to an S3 bucket with static hosting
- **Firebase Hosting**: Use Firebase CLI to deploy

## 📬 Contact Form Setup

### Option 1: Netlify Forms (Recommended for Netlify hosting)

1. The form is already configured for Netlify Forms
2. After deploying to Netlify, forms will automatically work
3. View submissions in Netlify dashboard under Forms
4. Optional: Set up email notifications in Netlify settings

### Option 2: Formspree Integration

1. Go to [formspree.io](https://formspree.io) and create an account
2. Create a new form and get your form ID
3. Update the form action in `index.html`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
4. Replace `YOUR_FORM_ID` with your actual Formspree form ID

### Option 3: Custom Backend

If you prefer a custom solution, you can:
- Set up a serverless function (Netlify Functions, Vercel API routes)
- Use a backend service like EmailJS
- Integrate with your existing CRM system

## 🎨 Customization

### Updating Contact Information

Edit these sections in `index.html`:

```html
<!-- Email links -->
<a href="mailto:hello@twomenandai.com">hello@twomenandai.com</a>

<!-- Phone number -->
<a href="tel:+15551234567">+1 (555) 123-4567</a>
```

### Changing Colors and Styling

The website uses a gradient color scheme. Main colors are defined in CSS:
- Primary: `#667eea` (blue)
- Secondary: `#764ba2` (purple)
- Accent: `white` and various grays

To change colors, find and replace these hex values in the `<style>` section.

### Adding/Modifying Services

Services are in the `.services-grid` section. Each service follows this structure:

```html
<div class="service-card">
    <div class="service-icon">🔧</div>
    <h3>Service Title</h3>
    <p>Service description...</p>
</div>
```

### Updating Company Statistics

Modify the stats in the about section:

```html
<div class="stat">
    <div class="stat-number">50+</div>
    <div class="stat-label">Projects Completed</div>
</div>
```

## 📱 Mobile Responsiveness

The website is fully responsive and optimized for:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (up to 767px)

All components automatically adapt to different screen sizes.

## 🔧 Technical Features

### Performance Optimizations
- Embedded CSS and JavaScript (no external dependencies)
- Optimized images and fonts
- Gzip compression via Netlify
- Browser caching headers

### SEO Features
- Semantic HTML structure
- Meta tags for search engines
- Open Graph tags for social sharing
- Structured data ready
- Fast loading times

### Security Features
- Content Security Policy headers
- XSS protection
- Frame options protection
- HTTPS enforcement

## 📊 Analytics Setup (Optional)

To add Google Analytics:

1. Get your GA4 tracking ID
2. Add before closing `</head>` tag:

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

## 🛠 Maintenance

### Regular Updates
- Review contact information quarterly
- Update project statistics as needed
- Refresh service descriptions annually
- Monitor form submissions regularly

### Content Updates
- See `docs/update-guide.md` for detailed instructions
- Most content can be updated by editing `index.html`
- Test changes locally before deploying

### Backup
- Keep regular backups of your customized files
- Use Git for version control
- Document any customizations you make

## 🆘 Troubleshooting

### Contact Form Not Working
1. Check browser console for JavaScript errors
2. Verify form action URL is correct
3. Ensure Formspree/Netlify Forms is properly configured
4. Test with simple email client if needed

### Website Not Loading
1. Check domain DNS settings for 2men.ai
2. Verify hosting service status
3. Clear browser cache
4. Check for JavaScript errors in console

### Mobile Display Issues
1. Test on multiple devices/browsers
2. Use browser developer tools to simulate devices
3. Check for CSS conflicts
4. Verify viewport meta tag is present

## 📞 Support

For technical support or customization help:
- Email: hello@twomenandai.com
- Check `docs/update-guide.md` for detailed instructions
- Review browser console for error messages

## 📝 License

This website template is provided as-is for Two Men and AI. Feel free to modify and customize as needed for your business requirements.

---

**Last Updated:** January 2024
**Version:** 1.0.0
**Tested On:** Chrome, Firefox, Safari, Edge