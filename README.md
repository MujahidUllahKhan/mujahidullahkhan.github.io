# Mujahid Ullah Khan Afridi — Personal Academic Website

A static HTML/CSS site (no build tools needed) with six pages: Home, Research, Publications, CV, Honors & Service, Contact.

## Structure
```
website/
├── index.html
├── research.html
├── publications.html
├── cv.html
├── honors.html
├── contact.html
├── assets/
│   ├── css/style.css
│   ├── js/main.js
│   ├── cv/Mujahid_Afridi_CV.pdf   <- swap in your latest CV anytime, same filename
│   └── img/                        <- add a headshot here, then update index.html
```

## Before going live — quick edits
1. **Add a photo**: drop a headshot into `assets/img/` and replace the "Add Photo" placeholder circle in `index.html` (`<div class="hero-photo">`) with `<img src="assets/img/your-photo.jpg" alt="Mujahid Ullah Khan Afridi">`.
2. **Dashboard link**: `research.html` has a placeholder "View Dashboard" link for the R/Shiny project — replace `href="#"` with the live URL once you have one (e.g. shinyapps.io).
3. **Update the CV**: replace `assets/cv/Mujahid_Afridi_CV.pdf` with a newer export whenever your CV changes — keep the same filename and the site updates automatically.
4. **Phone number**: left off the Contact page by default for privacy. Add it in `contact.html` if you want it public.

## How to make it live (free options)

### Option A — GitHub Pages (recommended, free, easiest to maintain)
1. Create a free GitHub account and a new repository, e.g. `mujahid-afridi.github.io` (using this exact name gives you a live site at `https://mujahid-afridi.github.io` with zero extra config).
2. Upload everything inside this `website/` folder to the root of that repository (drag-and-drop works on github.com, or use `git push`).
3. In the repo, go to **Settings → Pages**, set source to the `main` branch, root folder, and save.
4. Your site goes live at `https://<your-username>.github.io` within a few minutes.
5. Optional custom domain: buy a domain (e.g. from Namecheap/Google Domains, ~$10–15/yr) and add it under **Settings → Pages → Custom domain**.

### Option B — Netlify (free, drag-and-drop, no account setup needed for a quick preview)
1. Go to netlify.com, sign up free.
2. Drag the `website/` folder onto the Netlify dashboard ("Deploy manually").
3. You get a live URL instantly (e.g. `yourname.netlify.app`); you can rename the subdomain for free in Site Settings.
4. Optional custom domain can be added the same way as GitHub Pages.

### Option C — Vercel (similar to Netlify)
1. Go to vercel.com, sign up free, and use "Add New Project" → deploy the folder, or connect it to a GitHub repo for auto-deploys on every update.

## Recommended domain (optional, ~$10-15/year)
For NIW and academic credibility, a custom domain like `mujahidafridi.com` or `firstlast.dev` looks more professional than a subdomain. Buy from any registrar (Namecheap, Google Domains, Cloudflare Registrar) and point it at whichever host you choose above — happy to walk through DNS setup when you're ready.

## Updating content later
All pages are plain HTML — open any `.html` file in a text editor, edit the text between tags, save, and re-upload/re-deploy. No coding framework or build step required.
