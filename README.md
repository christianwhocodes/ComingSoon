# ComingSoon Jekyll Site 🚀

This is a simple, customizable "Coming Soon" website built with [Jekyll](https://jekyllrb.com/) and automatically deployed to GitHub Pages using GitHub Actions.

## ✨ Features

- Easy to update site content using GitHub Actions variables (no code changes needed!)
- Clean, modular structure (layouts, includes, data)
- Ready for GitHub Pages deployment

## 🛠️ Customizing Your Site

You can change your site’s title, description, hero text, contact info, and social links by setting repository variables in GitHub:

1. Go to your repo’s **Settings** → **Secrets and variables** → **Actions** → **Variables**.
2. Add or update these variables:

| Variable Name        | Example Value                        | Purpose                              |
|----------------------|--------------------------------------|--------------------------------------|
| SEO_TITLE            | My Awesome Website                   | Site title (for SEO)                 |
| SEO_DESCRIPTION      | The coolest website ever made!       | Site description (for SEO)           |
| SEO_KEYWORDS         | awesome, website, coming soon        | Site keywords (for SEO)              |
| SEO_AUTHOR           | Jane Doe                             | Site author (for SEO)                |
| HERO_TITLE           | Welcome to Awesomeness!              | Main hero section title              |
| HERO_SUBTITLE        | Where dreams come true!              | Main hero section subtitle           |
| HERO_NEWSLETTER_TEXT | Subscribe for updates!               | Hero section newsletter text         |
| FOOTER_COPYRIGHT     | All Rights Reserved                  | Footer copyright text                |
| FOOTER_CREDITS       | Designed by Jane Doe                 | Footer credits text                  |
| CONTACT_EMAIL        | hello@myawesome.com                  | Contact email                        |
| CONTACT_PHONE        | +1 555 AWESOME                       | Contact phone                        |
| ADDRESS_STREET       | 123 Main St                          | Address street                       |
| ADDRESS_CITY         | Springfield, USA                     | Address city                         |
| HOURS_WEEKDAYS       | 9AM - 5PM                            | Opening hours (weekdays)             |
| HOURS_WEEKEND        | Closed                               | Opening hours (weekend)              |
| SOCIAL_TWITTER       | https://twitter.com/myawesome        | Twitter link                         |
| SOCIAL_FACEBOOK      | https://facebook.com/myawesome       | Facebook link                        |
| SOCIAL_INSTAGRAM     | https://instagram.com/myawesome      | Instagram link                       |
| SOCIAL_LINKEDIN      | https://linkedin.com/in/myawesome    | LinkedIn link                        |
| COUNTDOWN_DATE       | 2025/12/3                            | Countdown date (YYYY/MM/DD)          |

If a variable is not set, a default value will be used.

## ⚙️ GitHub Pages Configuration

Before your site can be published, make sure to configure GitHub Pages correctly:

1. **Repository Visibility:**  
   Your repository must be **public** for GitHub Pages to deploy.

2. **Set Pages Source:**  
   Go to your repo’s **Settings** → **Pages**.  
   - Under **Build and deployment**, set **Source** to **GitHub Actions** (not from a branch).

3. **First Deployment:**  
   After pushing to `main`, the GitHub Actions workflow will build and deploy your site.  
   The published site URL will be shown in the Pages settings and in the Actions logs.

4. **Troubleshooting:**  
   - If you see a 404, wait a few minutes for GitHub Pages to process the deployment.
   - Ensure your workflow completed successfully and the repo is public.

## 🚀 Deploying

Just push to the `main` branch—GitHub Actions will build and publish your site automatically!

## 🧪 Testing Your Site Locally

You can preview your site on your computer before pushing changes.

### Option 1: Install Jekyll on Your Computer

#### Step 1: Install Ruby and Jekyll

**Windows (PowerShell as Administrator):**
```powershell
winget search ruby
winget install RubyInstallerTeam.RubyWithDevKit.3.2

# Add Ruby to your PATH (if not already added).
# Replace 'C:\Ruby32-x64\bin' with your actual Ruby install path if different

[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\Ruby32-x64\bin", [System.EnvironmentVariableTarget]::Machine)

# Restart your PowerShell terminal
# You may need to restart your PC if `gem` is not found
# Admin shell not necessary
gem install jekyll bundler
```

**Mac:**
```sh
brew install ruby
gem install jekyll bundler
```

**Linux (Ubuntu):**
```sh
sudo apt-get install ruby-full build-essential zlib1g-dev
gem install jekyll bundler
```

#### Step 2: In your project folder

```sh
# First time only
bundle install

# Every time you want to test
bundle exec jekyll serve
```

To use a different port (e.g., 3000):

```sh
bundle exec jekyll serve --port 3000
```

#### Step 3: Open your browser

Visit [http://localhost:4000](http://localhost:4000) (or your chosen port).

---

Happy building! 🌟