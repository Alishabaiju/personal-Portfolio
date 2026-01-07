# 📧 Contact Form Setup - Send Messages to Your Email

Your contact form is ready! You just need to connect it to Formspree (takes 2 minutes).

---

## ✅ Quick Setup (2 Minutes)

### Step 1: Create Formspree Account
1. Go to **[https://formspree.io](https://formspree.io)**
2. Click **"Sign Up"** (top right)
3. Sign up with Google, GitHub, or email (it's free!)

### Step 2: Create Your Form
1. After logging in, click **"+ New Form"** button
2. Give it a name: **"Portfolio Contact"**
3. Set **"Send submissions to"**: `alishabaiju2005@gmail.com`
4. Click **"Create Form"**

### Step 3: Get Your Form ID
1. After creating the form, you'll see your **Form ID**
2. It looks like: `xvgkqyzw` or `abc123xyz` (just letters/numbers)
3. **Copy this Form ID**

### Step 4: Update Your Code
1. Open `index.html` in your code editor
2. Find this line (around line 173):
   ```html
   <form class="contact-form" id="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
3. Replace `YOUR_FORM_ID` with your actual Form ID

**Example:**
If your Form ID is `xvgkqyzw`, change it to:
```html
<form class="contact-form" id="contact-form" action="https://formspree.io/f/xvgkqyzw" method="POST">
```

### Step 5: Test It!
1. Save `index.html`
2. Open it in your browser
3. Fill out the contact form
4. Click "Send Message"
5. Check your email inbox - you should receive the message!

---

## 🎯 What Happens When Someone Submits the Form?

1. User fills out the form and clicks "Send Message"
2. Formspree receives the message
3. Formspree sends an email to: **alishabaiju2005@gmail.com**
4. You receive the email with:
   - Sender's name
   - Sender's email
   - Their message
5. User sees a success message on your website

---

## 📊 Free Tier Limits

- **50 submissions per month** (perfect for a portfolio!)
- No credit card required
- Free forever

---

## ❓ Troubleshooting

**Form not sending?**
- Make sure you replaced `YOUR_FORM_ID` with your actual Form ID
- Check that there are no extra spaces in the URL
- Verify your email is set correctly in Formspree: `alishabaiju2005@gmail.com`

**Not receiving emails?**
- Check your spam folder
- Verify the email in Formspree settings is correct
- Make sure Formspree form is active (not paused)

**Need help?**
- Formspree documentation: [https://help.formspree.io](https://help.formspree.io)
- Or email me if you need assistance!

---

## ✨ That's It!

Once you replace `YOUR_FORM_ID` with your actual Form ID, your contact form will work perfectly and send all messages directly to your email inbox!

