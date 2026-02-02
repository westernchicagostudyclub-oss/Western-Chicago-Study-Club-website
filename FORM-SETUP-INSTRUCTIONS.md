# How to Set Up Contact Form (5 minutes)

## Your form is already configured! Just need to connect it to Formspree.

### Step 1: Sign Up for Formspree
1. Go to **https://formspree.io**
2. Click **"Get Started"** or **"Sign Up"**
3. Sign up using: **westernchicagostudyclub@gmail.com**
4. Check your email and verify your account

### Step 2: Create Your Form
1. Once logged in, click **"+ New Form"**
2. Name it: **"Contact Form"**
3. Click **"Create Form"**
4. You'll see a **Form Endpoint** that looks like: `https://formspree.io/f/xyzabc123`
5. **Copy the part after /f/** (example: `xyzabc123`)

### Step 3: Update Your Website
1. In GitHub, open **join.html**
2. Click the pencil icon to edit
3. Find this line at the top of the form (around line 67):
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
4. Replace `YOUR_FORM_ID` with your actual form ID
5. Example: `<form class="contact-form" action="https://formspree.io/f/xyzabc123" method="POST">`
6. Click **"Commit changes"**

### Step 4: Test It!
1. Wait 2 minutes for GitHub Pages to update
2. Go to your website: **westernchicagostudyclub.com/join.html**
3. Fill out the form and submit
4. Check **westernchicagostudyclub@gmail.com** for the submission!

---

## What the Form Does:

✅ Sends to: **westernchicagostudyclub@gmail.com**
✅ CC's: **horizonoms@outlook.com** (you'll get a copy too)
✅ Subject line: "New Contact from Western Chicago Study Club"
✅ Includes all form fields: name, email, phone, practice, specialty, etc.
✅ Spam protection built-in
✅ Works perfectly on mobile

---

## Formspree Free Plan:

- **50 submissions per month** (plenty for a study club)
- No ads
- Spam filtering included
- Email notifications
- Form dashboard to see all submissions

If you need more than 50/month later, paid plans start at $10/month.

---

## Alternative Option: Google Forms

If you'd prefer, you could also use Google Forms instead:
1. Create a form at **forms.google.com**
2. Set it to send responses to your email
3. Embed it in your website

But Formspree looks more professional and matches your site design!

---

## Troubleshooting:

**Form says "Confirm your email"** → Check westernchicagostudyclub@gmail.com for verification
**Submissions not arriving** → Check spam folder, verify form ID is correct
**Need help?** → Formspree has great support at help.formspree.io

---

That's it! Once you add your Formspree ID, the form will work perfectly.
