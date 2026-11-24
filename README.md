# Personal Portfolio Website

This is a simple, modern personal portfolio website built with **HTML** and **CSS**.  
It showcases:

- Self introduction
- Skills
- Contact form
- Responsive layout (works on mobile, tablet, and desktop)

## Features

- **Semantic HTML structure** using elements like `header`, `main`, `section`, and `footer`.
- **Clean, modern CSS styling** with a dark theme, custom typography, and subtle shadows.
- **Responsive design** using Flexbox, CSS Grid, and media queries.
- **Contact form** using EmailJS for reliable email delivery.

## Getting Started

1. **Open the project folder**
   - Navigate to this folder: `portfolio`.

2. **Open the website**
   - Double-click `index.html`  
   - Or right-click `index.html` → “Open with” → choose your browser (Chrome, Edge, etc.)

3. **View it on mobile**
   - Open the site in your browser.
   - Use the browser’s responsive design mode (e.g., F12 → “Toggle device toolbar” in Chrome)  
     or simply open the site on your phone (by hosting it or using Live Server in VS Code).

## Customize the Content

Open `index.html` in your code editor and update:

- **Name & Intro**
  - Change ` Name` in the hero section.
  - Edit the paragraph under “A passionate learner and aspiring web developer…” to describe yourself.

- **Skills**
  - In the `Skills` section, change the titles and descriptions to match your own skills.

- **Contact Form Setup (EmailJS)**
  - The contact form uses EmailJS to send emails directly to your inbox.
  - To set it up:
    1. Go to [EmailJS.com](https://www.emailjs.com/) and create a free account
    2. Create an Email Service (Gmail, Outlook, etc.) and get your **Service ID**
    3. Create an Email Template with these variables: `{{from_name}}`, `{{from_email}}`, `{{message}}`
    4. Get your **Template ID** and **Public Key**
    5. In `index.html`, replace these placeholders:
       - `YOUR_PUBLIC_KEY` with your EmailJS Public Key
       - `YOUR_SERVICE_ID` with your Service ID
       - `YOUR_TEMPLATE_ID` with your Template ID
    6. Update the recipient email in your EmailJS template settings to `xxxxxxxxxxxx@gmail.com`

## Customize the Style

Open `styles.css` to adjust:

- **Colors** – change the background and accent colors (for example, update `#0f172a`, `#020617`, `#38bdf8`, `#a855f7`).
- **Fonts** – update the `font-family` in the `body` rule.
- **Spacing** – tweak `padding`, `margin`, and `gap` values to fit your taste.

## Next Steps & Ideas

- Add a **Projects** section with cards for your best work.
- Include **social links** (GitHub, LinkedIn, etc.) in the header or footer.
- Add simple **scroll animations** with a bit of JavaScript or a lightweight library.

---
**Author:** Alisha Baiju  
**Project Type:** Frontend-only (HTML & CSS)

Enjoy building your portfolio!


