![](assets/img//social-preview.png)

# [Coming Soon](https://github.com/christianwhocodes/ComingSoon) 🚀

This is a simple, customizable "Coming Soon" website built with [Jekyll](https://jekyllrb.com/) and automatically deployed to GitHub Pages using GitHub Actions.

## ✨ Features

- Easy to update site content using GitHub Actions variables (no code changes needed!)
- Clean, modular structure (layouts, includes, data)
- Ready for GitHub Pages deployment

## 🪄 Use This Template for Your Own "Coming Soon" Site

You can easily create your own "Coming Soon" site by forking this repository and customizing it with your own content—no code changes required!

**Steps:**
1. **Fork this repository**  
   Click the "Fork" button at the top right of this page to create your own copy under your GitHub account.

2. **Customize via GitHub Actions Variables**  
   Go to your fork's **Settings** → **Secrets and variables** → **Actions** → **Variables** and set your site's title, description, hero text, contact info, social links, countdown date, and more ([see table below](#️-customizing-your-site)).

3. **Deploy**  
   Push to your `main` branch (or just save your variable changes). GitHub Actions will build and deploy your customized site automatically ([see GitHub Pages Configuration section below](#️-github-pages-configuration)).

4. **Update Anytime**  
   You can update your site's content at any time by changing the variables—no need to edit code or HTML!

## 🛠️ Customizing Your Site

You can change your site's title, description, hero text, contact info, social links, and more by setting repository variables in GitHub:

1. Go to your repo's **Settings** → **Secrets and variables** → **Actions** → **Variables**.
2. Add or update these variables:

| Variable Name        | Purpose                              | Default Value                                                                 | Example Value                        |
|----------------------|--------------------------------------|-------------------------------------------------------------------------------|--------------------------------------|
| SITE_TITLE           | Site title (for SEO)                 | Coming Soon                                                                  | My Awesome Website                   |
| SITE_DESCRIPTION     | Site description (for SEO)           | We are still working on our website. Stay tuned for updates!                 | The coolest website ever made!       |
| SITE_KEYWORDS        | Site keywords (for SEO)              | bootstrap, template, coming soon                                             | awesome, website, coming soon        |
| SITE_AUTHOR          | Site author (for SEO)                | Christian Who Codes                                                          | Kevin Wakhisi                        |
| ICONS_FAVICON_ICO    | Path or URL to favicon.ico           | assets/img/favicon.ico                                                       | https://example.com/favicon.ico      |
| ICONS_APPLE_TOUCH_ICON| Path or URL to Apple touch icon     | assets/img/apple-touch-icon.png                                              | https://example.com/apple-touch-icon.png |
| BACKGROUND_IMAGE     | Path or URL to background image      | assets/img/bg.jpg                                                            | https://example.com/bg.jpg           |
| HERO_TITLE           | Main hero section title              | Something Revolutionary is Coming                                            | Welcome to Awesomeness!              |
| HERO_SUBTITLE        | Main hero section subtitle           | We are still working on our website. Stay tuned for updates!                 | Where dreams come true!              |
| HERO_NEWSLETTER_TEXT | Hero section newsletter text         | Subscribe now to get the latest updates!                                     | Subscribe for updates!               |
| FOOTER_COPYRIGHT     | Footer copyright text                | All rights reserved.                                                         | All Rights Reserved                  |
| FOOTER_CREDITS       | Footer credits text                  | Crafted with ❤️ by <a href="https://github.com/christianwhocodes" target="_blank" rel="noopener"><em>Christian Who Codes</em></a> | Designed by Jane Doe                 |
| CONTACT_EMAIL        | Contact email                        | (none)                                                                       | hello@myawesome.com                  |
| CONTACT_PHONE        | Contact phone                        | (none)                                                                       | +254 777 AWESOME                     |
| ADDRESS_STREET       | Address street                       | (none)                                                                       | 00600 Ngara Rd                       |
| ADDRESS_CITY         | Address city                         | (none)                                                                       | Nairobi, Kenya                       |
| HOURS_WEEKDAYS       | Opening hours (weekdays)             | (none)                                                                       | 9AM - 5PM                            |
| HOURS_SATURDAY       | Opening hours (saturday)             | (none)                                                                       | 9AM - 5PM                            |
| HOURS_SUNDAY         | Opening hours (sunday)               | (none)                                                                       | Closed                               |
| SOCIAL_TWITTER       | Twitter link                         | (none)                                                                       | https://twitter.com/myawesome        |
| SOCIAL_FACEBOOK      | Facebook link                        | (none)                                                                       | https://facebook.com/myawesome       |
| SOCIAL_INSTAGRAM     | Instagram link                       | (none)                                                                       | https://instagram.com/myawesome      |
| SOCIAL_LINKEDIN      | LinkedIn link                        | (none)                                                                       | https://linkedin.com/in/myawesome    |
| COUNTDOWN_DATE       | Countdown date (YYYY/MM/DD)          | (none)                                                                       | 2025/12/3                            |

If a variable is not set, a default value will be used where shown above.

## 🚀 Deploying

Just push to the `main` branch—GitHub Actions will build and publish your site automatically!

## ⚙️ GitHub Pages Configuration

Before your site can be published, make sure to configure GitHub Pages correctly:

1. **Repository Visibility:**  
   Your repository must be **public** for GitHub Pages to deploy.

2. **Set Pages Source:**  
   Go to your repo's **Settings** → **Pages**.  
   - Under **Build and deployment**, set **Source** to **GitHub Actions** (not from a branch).

3. **First Deployment:**  
   After pushing to `main`, the GitHub Actions workflow will build and deploy your site.  
   The published site URL will be shown in the Pages settings and in the Actions logs.

4. **Troubleshooting:**  
   - If you see a 404, wait a few minutes for GitHub Pages to process the deployment.
   - Ensure your workflow completed successfully and the repo is public.