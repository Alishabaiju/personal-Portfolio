# EmailJS Setup Guide - Step by Step

This guide will help you set up EmailJS so your contact form can send emails to your inbox.

## What are these credentials?

- **Public Key**: A unique identifier that allows your website to connect to EmailJS
- **Service ID**: Identifies which email service (Gmail, Outlook, etc.) to use
- **Template ID**: Identifies which email template to use when sending emails

---

## Step-by-Step Setup

### Step 1: Create EmailJS Account

1. Go to [https://www.emailjs.com/](https://www.emailjs.com/)
2. Click **"Sign Up"** (top right)
3. Sign up with Google, GitHub, or email
4. Verify your email if needed

---

### Step 2: Get Your PUBLIC KEY

1. After logging in, click on your **profile/account icon** (top right)
2. Go to **"Account"** → **"General"** (or just click "Account" in the sidebar)
3. Scroll down to find **"Public Key"**
4. It looks like: `abcdefghijklmnop` (a string of letters/numbers)
5. **Copy this Public Key** - you'll need it for `YOUR_PUBLIC_KEY`

**Where to find it:**
- Dashboard → Account → General → Public Key section

---

### Step 3: Create an Email Service (Get SERVICE ID)

1. In the EmailJS dashboard, click **"Email Services"** in the left sidebar
2. Click the **"+ Add New Service"** button
3. Choose your email provider:
   - **Gmail** (recommended if you use Gmail)
   - **Outlook** (if you use Outlook/Hotmail)
   - Or any other provider
4. Follow the connection steps:
   - For Gmail: You'll need to connect your Google account
   - For Outlook: Connect your Microsoft account
5. Give your service a name (e.g., "Portfolio Contact Form")
6. Click **"Create Service"**
7. After creating, you'll see your **Service ID** - it looks like: `service_abc123` or `service_xyz789`
8. **Copy this Service ID** - you'll need it for `YOUR_SERVICE_ID`

**Where to find it:**
- Email Services → Your service name → Service ID (shown at the top or in settings)

---

### Step 4: Create an Email Template (Get TEMPLATE ID)

1. In the EmailJS dashboard, click **"Email Templates"** in the left sidebar
2. Click **"+ Create New Template"**
3. Fill in the template:
   - **Template Name**: "Portfolio Contact Form" (or any name)
   - **Subject**: `New message from {{from_name}}` (or customize)
   - **Content**: Use this template:

   ```
   You have a new message from your portfolio website!
   
   From: {{from_name}}
   Email: {{from_email}}
   
   Message:
   {{message}}
   ```

4. **Important**: Make sure to use these exact variable names:
   - `{{from_name}}` - sender's name
   - `{{from_email}}` - sender's email
   - `{{message}}` - the message content

5. Scroll down to **"To Email"** and enter: `alishabaiju2005@gmail.com`
6. **"From Name"** can be: `Portfolio Website` (or leave default)
7. Click **"Save"**
8. After saving, you'll see your **Template ID** - it looks like: `template_abc123` or `template_xyz789`
9. **Copy this Template ID** - you'll need it for `YOUR_TEMPLATE_ID`

**Where to find it:**
- Email Templates → Your template name → Template ID (shown at the top or in the URL)

---

### Step 5: Update Your Code

1. Open `index.html` in your code editor
2. Find line 229 (around there) - you'll see:
   ```javascript
   emailjs.init("YOUR_PUBLIC_KEY");
   ```
   Replace `YOUR_PUBLIC_KEY` with your actual Public Key

3. Find line 253 (around there) - you'll see:
   ```javascript
   emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", formData)
   ```
   Replace:
   - `YOUR_SERVICE_ID` with your Service ID
   - `YOUR_TEMPLATE_ID` with your Template ID

**Example of what it should look like:**
```javascript
emailjs.init("abcdefghijklmnop123456"); // Your Public Key

// ...

emailjs.send("service_abc123", "template_xyz789", formData) // Your Service ID and Template ID
```

---

## Quick Reference: Where to Find Each ID

| Credential | Where to Find |
|------------|---------------|
| **Public Key** | Account → General → Public Key |
| **Service ID** | Email Services → Your service → Service ID |
| **Template ID** | Email Templates → Your template → Template ID |

---

## Testing

1. Save your `index.html` file
2. Open it in a browser
3. Fill out the contact form
4. Click "Send Message"
5. Check your email inbox (`alishabaiju2005@gmail.com`) - you should receive the message!

---

## Troubleshooting

**Form not sending?**
- Double-check that all three IDs are correctly replaced (no quotes around them, no extra spaces)
- Make sure your email service is connected properly
- Check that the template variables match exactly: `{{from_name}}`, `{{from_email}}`, `{{message}}`

**Getting errors?**
- Open browser console (F12) to see error messages
- Make sure you're using the correct Service ID and Template ID
- Verify your Public Key is correct

---

## Free Tier Limits

EmailJS free tier includes:
- **200 emails per month** - Perfect for a portfolio site!
- No credit card required

---

Need help? Check EmailJS documentation: [https://www.emailjs.com/docs/](https://www.emailjs.com/docs/)

