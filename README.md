# Mackler Master Plumbing & Heating — Website

This folder contains the complete one-page website for **macklerplumbing.com**, ready to deploy.

---

## What's inside

- **`index.html`** — The full site (cover, services, about, clients, contact form, footer).
- **`styles.css`** — All visual styling (navy/gold heritage aesthetic, matches your letterhead).
- **`README.md`** — This file.

---

## Quick-start: Get the site online in 30 minutes

### Step 1 — Register the domain

1. Go to **[Namecheap.com](https://www.namecheap.com)** or **[GoDaddy.com](https://www.godaddy.com)**.
2. Search for `macklerplumbing.com`.
3. Register it. Expect **~$12–15/year**.
4. **Turn on "WHOIS privacy"** when checking out (free at Namecheap, sometimes a small fee at GoDaddy). This hides your personal address from public records.
5. **Decline upsells** — no need for "premium DNS," "email packages," etc. yet.

### Step 2 — Hook up the contact form (Formspree)

The contact form currently won't email you anything until you connect it.

1. Go to **[Formspree.io](https://formspree.io)** and create a free account.
2. Create a new form. Use `macklerfire@gmail.com` as the destination.
3. Formspree will give you a form URL like `https://formspree.io/f/abcd1234`.
4. Open **`index.html`** and find this line (around line 290):
   ```html
   <form class="form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
5. Replace `YOUR_FORM_ID` with your actual ID (e.g., `abcd1234`).
6. Save the file.

> **Free plan = 50 form submissions/month.** If you outgrow that, paid plans start at $10/month.

### Step 3 — Deploy with GitHub Pages (free hosting)

1. Create a free account at **[GitHub.com](https://github.com)**.
2. Create a new **public** repository named exactly **`macklerplumbing.com`** (or anything you like).
3. Upload `index.html` and `styles.css` to the repo (drag and drop on the GitHub website is fine).
4. Go to repo **Settings → Pages**.
5. Under "Source," choose **"Deploy from a branch"**, branch = **`main`**, folder = **`/ (root)`**. Click **Save**.
6. Wait ~2 minutes. Your site will be live at `https://yourusername.github.io/macklerplumbing.com`.

### Step 4 — Point your domain at GitHub Pages

1. In the same GitHub Pages settings, under **"Custom domain,"** enter `macklerplumbing.com` and click Save.
2. Check the **"Enforce HTTPS"** box (free, automatic).
3. Go back to your domain registrar (Namecheap/GoDaddy) and set these **DNS records**:

   | Type  | Host | Value             |
   |-------|------|-------------------|
   | A     | @    | 185.199.108.153   |
   | A     | @    | 185.199.109.153   |
   | A     | @    | 185.199.110.153   |
   | A     | @    | 185.199.111.153   |
   | CNAME | www  | yourusername.github.io |

4. Wait 10–60 minutes for DNS to propagate. Visit `macklerplumbing.com` and it's live.

---

## Customizing the site

### Change phone, email, or address

Search `index.html` for:
- `718-837-2868` — phone number
- `macklerfire@gmail.com` — email
- `7216 16th Avenue` — office address

Replace as needed. They appear in the top bar, hero buttons, contact section, and footer.

### Change colors

In `styles.css`, the top of the file has all colors as CSS variables:

```css
--navy:        #0D2B4E;   /* main brand navy */
--gold:        #B8860B;   /* accent gold */
--cream:       #F5F1E8;   /* warm cream background */
```

Change those values and the whole site updates automatically.

### Add or remove services

Find the `<section class="services">` block in `index.html`. Each service is an `<article class="svc">`. Copy/edit/delete as needed.

### Update client names or projects

Find the `<section class="trust">` block. The three "proj" articles list the named projects; the bottom row lists the C&W / CBRE / Related mention.

### Get a professional email (later)

When you're ready, set up `info@macklerplumbing.com` via **Google Workspace** ($7/user/month) or use the registrar's free email forwarding. Then update the email everywhere in `index.html`.

---

## Going beyond a one-page site (later)

When you're ready for more:
- **Add pages** (a dedicated Fire Suppression page, a Service Areas page, a Projects gallery, etc.).
- **Add Google Analytics** to see who's visiting.
- **Add Google Business Profile** — free, gets you on Google Maps for local plumbing searches. Huge for lead generation.
- **SEO**: Add page titles, meta descriptions, and structured data so you rank for "NYC plumber," "Brooklyn fire suppression," etc.

I can help with any of those when you're ready.

---

## Questions or changes

This site is set up to grow with the business. Anytime you need updates — new clients to add, services to revise, new pages, anything — just let me know.

— Built for **Mackler Master Plumbing & Heating Inc.** · Established 1985
