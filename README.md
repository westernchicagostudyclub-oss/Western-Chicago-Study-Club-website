# Western Chicago Study Club Website

## Overview
This is a professional, multi-page website for the Western Chicago Study Club, founded by Dr. Ali Al-Qudsi, Dr. Nader Amiran, and Dr. Mohammed Al Rubaie.

## Website Structure
- **index.html** - Homepage with welcome message and study club overview
- **about.html** - Detailed information about mission, vision, and what the club offers
- **founders.html** - Bios and photos of the three founding doctors
- **join.html** - Contact form and information for prospective members
- **styles.css** - Complete styling for all pages

## Setup Instructions

### Option 1: GitHub Pages (Recommended - FREE)

1. **Create a GitHub account** (if you don't have one)
   - Go to github.com and sign up

2. **Create a new repository**
   - Click the "+" icon → "New repository"
   - Name it: `western-chicago-study-club`
   - Make it Public
   - Click "Create repository"

3. **Upload the files**
   - Click "uploading an existing file"
   - Drag and drop all 5 files (index.html, about.html, founders.html, join.html, styles.css)
   - Click "Commit changes"

4. **Enable GitHub Pages**
   - Go to Settings → Pages
   - Under "Source", select "main" branch
   - Click Save
   - Your site will be live at: `https://yourusername.github.io/western-chicago-study-club/`

5. **Connect your Cloudflare domain**
   - In GitHub Pages settings, add custom domain: `westernchicagostudyclub.com`
   - In Cloudflare DNS, add CNAME record:
     - Type: CNAME
     - Name: www
     - Target: yourusername.github.io
   - Add another CNAME for root domain:
     - Type: CNAME
     - Name: @
     - Target: yourusername.github.io

### Option 2: Netlify (Also FREE)

1. **Go to netlify.com** and sign up
2. **Drag and drop** all website files into Netlify
3. **Connect custom domain** in site settings
4. **Update Cloudflare DNS** to point to Netlify

### Option 3: Simple Hosting

Upload all files to any web hosting provider via FTP.

## Customization

### Adding Photos
Replace the placeholder sections in `founders.html` with actual images:
```html
<!-- Replace this: -->
<div class="founder-image-placeholder">
    <div class="placeholder-content">
        <p>Dr. Ali Al-Qudsi Photo</p>
        <small>Photo to be added</small>
    </div>
</div>

<!-- With this: -->
<img src="path-to-photo.jpg" alt="Dr. Ali Al-Qudsi" style="width: 300px; height: 300px; border-radius: 10px; object-fit: cover;">
```

### Setting Up the Contact Form
The contact form in `join.html` needs a backend service. Two easy options:

**Option 1: Formspree (FREE for 50 submissions/month)**
1. Go to formspree.io and sign up
2. Create a new form
3. Copy your form endpoint
4. In `join.html`, replace `YOUR_FORM_ID` with your actual Formspree ID:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

**Option 2: Netlify Forms (FREE with Netlify hosting)**
Simply add `netlify` attribute to the form tag:
```html
<form class="contact-form" name="contact" method="POST" netlify>
```

### Updating Contact Information
Edit the email address in `join.html`:
```html
Email: <a href="mailto:info@westernchicagostudyclub.com">info@westernchicagostudyclub.com</a>
```

### Changing Colors
Edit the colors in `styles.css` at the top:
```css
:root {
    --primary-color: #1e4d7b;      /* Dark blue */
    --secondary-color: #2c7bb6;    /* Medium blue */
    --accent-color: #4a9fd8;       /* Light blue */
}
```

## Features
- Fully responsive (works on mobile, tablet, desktop)
- Professional design with clean typography
- Easy navigation between pages
- Contact form for prospective members
- Detailed founder bios
- SEO-friendly structure

## Support
If you need help setting this up, the founders can reach out to:
- GitHub Pages documentation: docs.github.com/pages
- Netlify documentation: docs.netlify.com
- Formspree documentation: help.formspree.io

## Future Enhancements
Consider adding:
- Actual founder photos
- Meeting calendar/schedule
- Member login area
- Photo gallery from events
- Newsletter signup
- Social media links
