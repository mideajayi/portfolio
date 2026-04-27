# Mide Ajayi — Portfolio

Personal portfolio website. Dark, minimal, typographic.

## Structure

```
/
├── index.html          — Homepage
├── about.html          — About page
├── work/
│   ├── fasttrack.html
│   ├── nobcredit.html
│   ├── send-onboarding.html
│   ├── send-referral.html
│   ├── raenest-wrapped.html
│   └── dca-calculator.html
├── assets/
│   ├── David_Ajayi_CV.pdf     ← ADD YOUR CV HERE
│   └── images/
│       └── projects/          ← ADD COVER IMAGES HERE
├── netlify.toml
└── vercel.json
```

## Before deploying

1. Add your CV PDF to `/assets/David_Ajayi_CV.pdf`
2. Add cover images to `/assets/images/projects/`
3. Replace placeholder divs with `<img>` tags in case study pages

## Adding cover images

In each case study page, find:
```html
<div class="cs-cover fade-in">
  <span class="cs-cover__placeholder">FastTrack — Cover image</span>
</div>
```

Replace with:
```html
<div class="cs-cover fade-in">
  <img src="../assets/images/projects/fasttrack-cover.jpg" alt="FastTrack by Mide Ajayi">
</div>
```

## Adding screen images

In the body sections, find:
```html
<div class="cs-screen fade-in">
  <span class="cs-screen__label">Final screens — key flow</span>
</div>
```

Replace with:
```html
<div class="cs-screen fade-in">
  <img src="../assets/images/projects/fasttrack-screens-01.jpg" alt="FastTrack final screens">
</div>
```

## Deploying to Netlify (recommended)

1. Create a GitHub repository
2. Push this folder to the repo
3. Go to netlify.com → New site from Git
4. Connect the repo — Netlify auto-detects netlify.toml
5. Add your custom domain in Site Settings → Domain Management

## Deploying to Vercel

1. Push to GitHub
2. Go to vercel.com → New Project
3. Import the repo — Vercel auto-detects vercel.json
4. Add custom domain in Project Settings → Domains

## Custom domain

Recommended: themideajayi.com or mideajayi.com
Point DNS to Netlify/Vercel nameservers after purchasing.

## Updating content

All content is in plain HTML — find the text, change it, commit and push.
No build step, no framework, no compilation needed.
