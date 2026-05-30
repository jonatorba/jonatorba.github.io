# Analytics Portfolio — GitHub Pages

A professional data analytics portfolio site built to showcase Power BI projects.

## 🚀 How to deploy (10 minutes)

### Step 1 — Create a GitHub repository
1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **New repository**
3. Name it exactly: `YOUR-USERNAME.github.io` (replace with your real GitHub username)
4. Set it to **Public**
5. Click **Create repository**

### Step 2 — Upload the site
1. On the new repo page, click **Add file → Upload files**
2. Drag and drop `index.html` into the upload area
3. Click **Commit changes**

### Step 3 — Enable GitHub Pages
1. Go to your repo **Settings → Pages**
2. Under "Source", select **Deploy from a branch**
3. Choose branch: **main**, folder: **/ (root)**
4. Click **Save**

Your site will be live at `https://YOUR-USERNAME.github.io` within 1–2 minutes.

---

## ✏️ Customization checklist

Open `index.html` in any text editor and find these sections (marked with ✏️ comments):

### Personal info
- [ ] `<span class="nav-name">Your Name · Analytics</span>` — update your name
- [ ] Hero headline and description paragraph
- [ ] About section bio (3 paragraphs)
- [ ] Skills tags in the 4 skill cards
- [ ] Footer name
- [ ] Stats strip numbers (projects, domains, visuals, datasets)

### Contact links
- [ ] LinkedIn URL and handle
- [ ] Email address (2 places)
- [ ] GitHub URL and handle

### Projects
Each project card has 4 things to update:
- [ ] `project-domain` label and color
- [ ] `project-name` title
- [ ] `project-desc` description
- [ ] `href="YOUR_POWER_BI_LINK_HERE"` → paste your Power BI "Publish to web" URL

### Adding more projects
Copy any `.project-card` block and paste it before the placeholder card.
Update the thumb gradient colors to match the domain color:
- Finance → blue (`#E6F1FB` to `#B5D4F4`)
- Sales → green (`#EAF3DE` to `#C0DD97`)
- Operations → amber (`#FAEEDA` to `#FAC775`)
- HR / People → purple (`#EEEDFE` to `#AFA9EC`)

---

## 📬 Making the contact form work

The form currently shows a success animation but doesn't send emails.
To wire it up for real, use **Formspree** (free tier, no backend needed):

1. Go to [formspree.io](https://formspree.io) and create a free account
2. Create a new form — copy your form endpoint URL (looks like `https://formspree.io/f/xxxxxxxx`)
3. In `index.html`, find the `<div class="contact-form">` section
4. Replace `<div class="contact-form">` with `<form class="contact-form" method="POST" action="YOUR_FORMSPREE_URL">`
5. Add `name="fname"`, `name="lname"`, `name="email"`, `name="message"` attributes to each input/textarea
6. Change `<button class="form-submit" onclick="handleSubmit(event)">` to `<button class="form-submit" type="submit">`

---

## 🔗 Getting Power BI "Publish to web" links

1. Open your report in Power BI Service
2. Click **File → Embed report → Publish to web (public)**
3. Confirm and copy the public URL
4. Paste it into the `href` of the matching project card

> ⚠️ Note: "Publish to web" makes reports publicly accessible without login.
> For reports with sensitive data, consider sharing via a workspace link instead
> and adding a note that viewers need Power BI access.

---

## 🎨 Design tokens (quick reference)

| Role | Value |
|---|---|
| Primary blue | `#185FA5` |
| Light blue | `#378ADD` |
| Positive | `#3B6D11` |
| Negative | `#A32D2D` |
| Warning | `#854F0B` |
| Body font | DM Sans |
| Display font | DM Serif Display |
