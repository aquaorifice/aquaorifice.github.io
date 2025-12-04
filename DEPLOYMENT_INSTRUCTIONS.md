# Deployment Instructions

## GitHub Actions Setup Complete! ✅

Your site now has automatic deployment via GitHub Actions. Every time you push to the `master` branch, GitHub will automatically build and deploy your Jekyll site.

---

## How It Works

1. **You push changes** to GitHub
2. **GitHub Actions automatically**:
   - Sets up Ruby and Jekyll
   - Installs dependencies from your Gemfile
   - Builds your Jekyll site
   - Deploys to GitHub Pages
3. **Your site updates** at https://aquaorifice.github.io/

---

## Enable GitHub Actions (One-Time Setup)

You need to configure GitHub Pages to use GitHub Actions:

1. Go to your repository: https://github.com/aquaorifice/aquaorifice.github.io
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Build and deployment":
   - **Source**: Select "GitHub Actions" (not "Deploy from a branch")
4. Save

That's it! Future pushes will automatically trigger the workflow.

---

## View Build Status

- Go to the **Actions** tab in your repository
- You'll see each deployment run
- Green checkmark = successful deployment
- Red X = build failed (check logs for errors)

---

## BU Website Redirect Setup

To redirect your BU website (cs-people.bu.edu/anwesha/) to your new GitHub Pages site:

### Step 1: Upload Redirect File

```bash
# Upload the redirect HTML as your main index.html
scp bu_redirect.html yourusername@csa2.bu.edu:~/public_html/index.html

# Or if you want to keep your BU site and just add a link:
scp bu_redirect.html yourusername@csa2.bu.edu:~/public_html/redirect.html
```

### Step 2: Set Permissions

```bash
ssh yourusername@csa2.bu.edu
chmod 644 ~/public_html/index.html
```

### Step 3: Test

Visit cs-people.bu.edu/anwesha/ - it should redirect to your GitHub Pages site!

---

## Making Updates to Your Site

### Method 1: Direct Editing (Recommended)

```bash
# Make your changes to files
cd /Users/anweshasaha/Desktop/anwesha-docs/anwesha.github.io

# Test locally first
/opt/homebrew/opt/ruby/bin/bundle exec jekyll serve
# Visit http://localhost:4000 to preview

# When satisfied, commit and push
git add .
git commit -m "Update: describe your changes"
git push origin master
```

GitHub Actions will automatically build and deploy in 2-3 minutes!

### Method 2: Quick Updates

For small text changes, you can edit directly on GitHub:
1. Navigate to the file on github.com
2. Click the pencil icon to edit
3. Commit changes
4. GitHub Actions builds automatically!

---

## Workflow File Location

The GitHub Actions workflow is located at:
```
.github/workflows/jekyll.yml
```

This file tells GitHub how to build your site. You generally don't need to modify it.

---

## Benefits of GitHub Actions

✅ **No manual building** - Just push and it deploys
✅ **Consistent builds** - Same environment every time
✅ **Build logs** - See exactly what happened if something fails
✅ **Automatic** - Works even if you edit on GitHub web interface
✅ **Version controlled** - The workflow is part of your repo

---

## Troubleshooting

### Build Fails
1. Check the Actions tab for error messages
2. Common issues:
   - Syntax errors in markdown or HTML
   - Missing gems in Gemfile
   - YAML formatting errors in _config.yml

### Site Not Updating
1. Wait 2-3 minutes after push
2. Hard refresh browser (Cmd+Shift+R on Mac)
3. Check Actions tab to ensure build succeeded
4. Verify GitHub Pages source is set to "GitHub Actions"

### Local Build vs GitHub Actions
- Always test locally first with `bundle exec jekyll serve`
- If it works locally, it should work on GitHub Actions
- Check that your Gemfile matches your local Ruby version

---

## Files You Modified

- `_config.yml` - Site configuration
- `index.html` - Homepage with news section
- `about.md` - About page
- `publications.md` - Publications page
- `experience.md` - Experience page
- `_sass/_base.scss` - Color theme (maroon)
- `_sass/_layout.scss` - Layout and styling
- `.github/workflows/jekyll.yml` - Deployment automation (NEW!)
- `bu_redirect.html` - BU website redirect page (NEW!)

---

## Quick Reference

### Deploy Changes
```bash
git add .
git commit -m "Your message"
git push origin master
```

### Test Locally
```bash
bundle exec jekyll serve
```

### View Live Site
https://aquaorifice.github.io/

### View Build Status
https://github.com/aquaorifice/aquaorifice.github.io/actions

---

## Next Steps

1. ✅ Push the GitHub Actions workflow file
2. ✅ Configure GitHub Pages to use Actions
3. ✅ Upload redirect to BU webspace
4. ✅ Test that everything works!

---

Last Updated: December 4, 2025

