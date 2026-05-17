# GitHub + Vercel Deployment Guide

## 1. Create GitHub Repository

Repository name:

`london-secret-of-women-site`

Description:

`Official coming-soon website for London – The Secret of Women, a cosmetics, beauty and wellness brand.`

Recommended settings:

- Public or Private: Public is easier for Vercel deployment
- Add README: No, because this package already includes README.md
- Add .gitignore: No, because this package already includes .gitignore
- Add license: Optional. Use proprietary/private if this is a commercial brand website.

## 2. Upload Files

Upload all files in this folder to the repository root:

- index.html
- london-secret-of-women-square-banner.png
- london-secret-of-women-wide-banner.png
- README.md
- DEPLOYMENT.md
- vercel.json
- .gitignore

## 3. Connect to Vercel

In Vercel:

1. Add New Project
2. Import GitHub repository: `london-secret-of-women-site`
3. Framework Preset: Other
4. Build Command: leave empty
5. Output Directory: leave empty
6. Deploy

## 4. Add Domain

In Vercel Project Settings → Domains, add:

`www.london-thesecretofwomen.com`

Optional root domain:

`london-thesecretofwomen.com`

## 5. DNS Records

If using Cloudflare or your domain registrar DNS:

For `www`:

Type: CNAME  
Name: www  
Target: cname.vercel-dns.com

For root domain:

Type: A  
Name: @  
Value: 76.76.21.21

## 6. Final Check

Open:

https://www.london-thesecretofwomen.com/

Check:

- Page loads correctly
- Banner images display
- Mobile layout works
- Contact/notify button opens email client
- HTTPS is active
