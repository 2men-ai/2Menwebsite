# Website Update Guide - Two Men and AI

This guide explains how to make common changes to your Two Men and AI website without technical expertise.

## 🎯 Quick Reference

| What to Update | File Location | Section |
|---|---|---|
| Contact Information | `index.html` | Multiple sections |
| Services | `index.html` | Services section |
| Company Stats | `index.html` | About section |
| Colors/Design | `index.html` | CSS style section |
| Contact Form | `index.html` | Contact section |

## 📞 Updating Contact Information

### Email Address
Find and replace all instances of `hello@twomenandai.com`:

**Line ~45** (Meta tags):
```html
<meta name="author" content="Two Men and AI">
```

**Line ~124** (Hero section button):
```html
<a href="mailto:hello@twomenandai.com" class="btn btn-secondary">Email Us</a>
```

**Line ~242** (Contact section):
```html
<li>📧 <a href="mailto:hello@twomenandai.com">hello@twomenandai.com</a></li>
```

### Phone Number
Find and replace `+1 (555) 123-4567`:

**Line ~243** (Contact section):
```html
<li>📞 <a href="tel:+15551234567">+1 (555) 123-4567</a></li>
```

*Note: In the `href`, remove spaces and special characters (keep +15551234567)*

### Company Name
To change "Two Men and AI" throughout the site:
1. Use Find & Replace in your text editor
2. Replace all instances of "Two Men and AI"
3. Update the logo text around line ~106

## 🛠 Updating Services

Services are located around line ~150. Each service follows this pattern:

```html
<div class="service-card">
    <div class="service-icon">⚙️</div>
    <h3>Service Title</h3>
    <p>Service description text here.</p>
</div>
```

### To Add a New Service:
1. Copy the entire `<div class="service-card">...</div>` block
2. Paste it before the closing `</div>` of `services-grid`
3. Update the emoji, title, and description

### To Remove a Service:
1. Delete the entire `<div class="service-card">...</div>` block

### Service Icons (Emojis):
- ⚙️ Legacy Systems
- 🗃️ Database
- 🤖 AI/Automation
- 💻 Software
- 📊 Analytics
- 🔗 Integration
- 🏭 Manufacturing
- 🔧 Tools
- ⚡ Performance
- 🎯 Strategy

## 📊 Updating Company Statistics

Statistics are around line ~220. Each stat follows this pattern:

```html
<div class="stat">
    <div class="stat-number">50+</div>
    <div class="stat-label">Manufacturing Projects</div>
</div>
```

### Common Stat Ideas:
- Projects Completed
- Years Experience
- Client Satisfaction %
- Industries Served
- Systems Modernized
- Cost Savings %

## 🎨 Changing Colors and Branding

### Main Colors
The website uses these primary colors:
- **Primary Blue**: `#667eea`
- **Secondary Purple**: `#764ba2`

To change colors, find and replace these hex codes in the CSS section (lines ~50-350).

### Logo Text
Update around line ~106:
```html
<div class="logo">Your Company Name</div>
```

### Favicon
To add a custom favicon:
1. Create a 32x32 pixel .ico file
2. Add this line in the `<head>` section:
```html
<link rel="icon" href="favicon.ico" type="image/x-icon">
```

## 📝 Updating Page Content

### Hero Section (Top of page)
Around line ~115:

```html
<h1>Transform Your Manufacturing with AI</h1>
<p>Your compelling subtitle here</p>
```

### About Section
Around line ~200:

```html
<h2>Manufacturing Technology Experts</h2>
<p>Your company description here...</p>
```

### Page Title and Meta Description
Around line ~10:

```html
<title>Your Page Title</title>
<meta name="description" content="Your page description for search engines">
```

## 📬 Contact Form Configuration

### Form Fields
The contact form (around line ~250) includes:
- Name (required)
- Company (required)
- Email (required)
- Phone (optional)
- Timeline (dropdown)
- Project Description (required)

### To Add/Remove Fields:

**Add a field:**
```html
<div class="form-group">
    <label for="fieldname">Field Label</label>
    <input type="text" id="fieldname" name="fieldname">
</div>
```

**Timeline Options:**
Update the `<select>` dropdown around line ~270:
```html
<option value="immediate">Immediate (1-2 weeks)</option>
<option value="short">Short-term (1-3 months)</option>
```

### Form Processing Setup

**Option 1: Netlify Forms (Recommended)**
- No changes needed if hosting on Netlify
- Forms automatically work after deployment

**Option 2: Formspree**
1. Go to [formspree.io](https://formspree.io)
2. Create an account and new form
3. Replace line ~250:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## 🔧 Testing Your Changes

### Before Publishing:
1. **Backup**: Save a copy of your original file
2. **Test Locally**: Open `index.html` in your browser
3. **Check Mobile**: Use browser developer tools to test mobile view
4. **Test Forms**: Try submitting the contact form
5. **Validate**: Check that all links work

### Common Issues:
- **Broken Layout**: Usually caused by missing closing tags `</div>`
- **Contact Form Not Working**: Check form action URL
- **Images Not Loading**: Verify file paths
- **Mobile Issues**: Test on actual devices

## 📱 Mobile Optimization

The website automatically adapts to mobile devices. Key breakpoints:
- **Desktop**: 1200px and up
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

No additional changes needed for mobile compatibility.

## 🔍 SEO Optimization

### Page Title
```html
<title>Your Company - What You Do | Location</title>
```

### Meta Description
```html
<meta name="description" content="Brief description (150-160 characters) with key benefits">
```

### Keywords
Update around line ~12:
```html
<meta name="keywords" content="your, main, keywords, here">
```

## 🚀 Publishing Changes

### If Using Netlify:
1. Save your changes to `index.html`
2. If connected to Git: Commit and push changes
3. If using drag & drop: Re-upload the file to Netlify
4. Changes go live automatically

### If Using Other Hosting:
1. Upload the modified `index.html` file
2. Replace the existing file on your server
3. Clear any caches if needed

## 📞 Getting Help

### Common Resources:
- **HTML Basics**: [W3Schools HTML Tutorial](https://www.w3schools.com/html/)
- **CSS Basics**: [W3Schools CSS Tutorial](https://www.w3schools.com/css/)
- **Formspree Help**: [Formspree Documentation](https://help.formspree.io/)
- **Netlify Help**: [Netlify Documentation](https://docs.netlify.com/)

### Professional Help:
If you need assistance with major changes:
- Contact a web developer
- Use freelancer platforms like Upwork or Fiverr
- Reach out to Two Men and AI for technical support

## ✅ Maintenance Checklist

### Monthly:
- [ ] Check that contact form is working
- [ ] Verify all links work correctly
- [ ] Update company statistics if needed
- [ ] Review and update service descriptions

### Quarterly:
- [ ] Update contact information
- [ ] Refresh project statistics
- [ ] Review and update meta descriptions
- [ ] Check mobile display on various devices

### Annually:
- [ ] Major content review and updates
- [ ] Consider design refresh
- [ ] Update copyright year in footer
- [ ] Review and update service offerings

---

**Need Help?** Contact hello@twomenandai.com for technical assistance.

**Last Updated:** January 2024