# Nico Padilla Personal Training — Website

Static website for Nico Padilla, a personal trainer in San Antonio, TX specializing in strength training and senior fitness.

**Live site:** [nicopadilla.com](https://nicopadilla.com)

## Setup: GitHub Pages + Custom Domain

### 1. Create the GitHub Repository
1. Go to [github.com/new](https://github.com/new)
2. Name the repository `nico-padilla-fitness`
3. Set it to **Public**
4. Push this code to the repository

### 2. Enable GitHub Pages
1. Go to the repo **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose the `main` branch and `/ (root)` folder
4. Click **Save**

### 3. Connect Custom Domain (nicopadilla.com)
1. In the repo **Settings** → **Pages**, enter `nicopadilla.com` under **Custom domain**
2. At your domain registrar, add these DNS records:

   **For apex domain (nicopadilla.com):**
   | Type | Name | Value |
   |------|------|-------|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |

   **For www subdomain:**
   | Type | Name | Value |
   |------|------|-------|
   | CNAME | www | YOUR_GITHUB_USERNAME.github.io |

3. Wait for DNS propagation (can take up to 24-48 hours)
4. Back in GitHub Pages settings, check **Enforce HTTPS**

### 4. Set Up the Contact Form (Formspree)
1. Go to [formspree.io](https://formspree.io) and create a free account
2. Create a new form and copy the form endpoint (e.g., `https://formspree.io/f/xabcdefg`)
3. In `index.html`, replace `YOUR_FORM_ID` in the form action URL with your actual form ID

## Customization Checklist

After deploying, update these placeholder items in `index.html`:

- [ ] **Hero image** — Add a background image to the hero section (update CSS in `style.css`)
- [ ] **About bio** — Replace placeholder text with Nico's real bio
- [ ] **Photo** — Replace the photo placeholder with an actual image
- [ ] **Certifications** — Update with real certification names
- [ ] **Testimonials** — Replace placeholder quotes with real client testimonials
- [ ] **Phone number** — Replace `(210) 555-1234` with real number
- [ ] **Email** — Replace `nico@example.com` with real email
- [ ] **Formspree form ID** — Replace `YOUR_FORM_ID` with actual Formspree endpoint

## Files

| File | Description |
|------|-------------|
| `index.html` | Main page with all content sections |
| `style.css` | All styles, responsive design included |
| `CNAME` | Created automatically by GitHub when custom domain is set |
