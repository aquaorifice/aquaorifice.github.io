# Anwesha Saha - Academic Portfolio Website

A modern, professional academic website showcasing research, publications, and professional experience.

## 🌟 Features

- **Clean White Design** with subtle animations and gradients
- **Responsive Layout** that works on all devices
- **News Highlights Section** featuring recent achievements
- **Publications Page** for research papers
- **Experience Section** highlighting Oracle work and PhD research
- **Portfolio** showcasing projects and talks
- **CV Page** with downloadable resume
- **Smooth Animations** including fade-ins, hover effects, and transitions

## 🚀 Quick Start

### Prerequisites
- Ruby (2.7 or higher)
- Jekyll
- Bundler

### Installation

```bash
# Install Jekyll and Bundler
gem install jekyll bundler

# Navigate to the site directory
cd /Users/anweshasaha/Desktop/anwesha-docs/anwesha.github.io

# Install dependencies
bundle install

# Run local server
bundle exec jekyll serve

# Visit http://localhost:4000 in your browser
```

## 📝 Customization Guide

See detailed guides:
- **QUICK_START.md** - Fast setup for your interview
- **SETUP_INSTRUCTIONS.md** - Complete deployment guide
- **CONTENT_EXAMPLES.md** - Examples and templates for content

### Essential Files to Update

1. **`_config.yml`** - Site settings, email, social media
2. **`index.html`** - Homepage with news highlights
3. **`about.md`** - Your biography and background
4. **`publications.md`** - Your research papers
5. **`experience.md`** - Work experience and skills
6. **`portfolio.md`** - Projects and achievements
7. **`cv.md`** - Complete CV
8. **`/img/prof_pic.jpg`** - Your profile picture

## 🎨 Design System

### Colors
- **Primary**: Dark Blue (`#00008B`)
- **Background**: White with subtle blue gradients
- **Accent**: Light Blue (`#e6f2ff`)
- **Text**: Dark Gray (`#333`)

### Typography
- **Font**: Helvetica, Arial, sans-serif
- **Base Size**: 16px
- **Headings**: Light weight (100-300)

### Animations
- Fade-in on page load
- Slide-in for news items
- Hover effects on cards
- Smooth transitions throughout

## 📂 Project Structure

```
anwesha.github.io/
├── index.html              # Homepage
├── about.md               # About page
├── publications.md        # Publications
├── experience.md          # Experience
├── portfolio.md           # Portfolio
├── cv.md                  # CV
├── _config.yml           # Site configuration
├── _includes/
│   ├── header.html       # Navigation
│   ├── footer.html       # Footer
│   └── head.html         # HTML head
├── _layouts/
│   ├── default.html      # Default layout
│   ├── page.html         # Page layout
│   └── post.html         # Post layout
├── _sass/
│   ├── _base.scss       # Base styles
│   ├── _layout.scss     # Layout and animations
│   └── _syntax-highlighting.scss
├── css/
│   └── main.scss         # Main stylesheet
├── img/                  # Images
└── js/                   # JavaScript files
```

## 🌐 Deployment

### To Boston University Server

```bash
# Build the site
bundle exec jekyll build

# Deploy to BU
scp -r _site/* your-username@cs-people.bu.edu:~/public_html/

# Or use rsync for incremental updates
rsync -avz --delete _site/ your-username@cs-people.bu.edu:~/public_html/
```

### To GitHub Pages (Alternative)

1. Push to GitHub
2. Enable GitHub Pages in repository settings
3. Select main branch
4. Site will be available at `https://username.github.io`

## ✨ Key Features Explained

### Homepage News Section
- Displays recent achievements
- Animated slide-in effects
- Easy to update with new items
- Links to external resources

### Publications Page
- Professional paper layout
- Award badges (like your Honorable Mention)
- Links to PDFs, slides, code
- Hover effects on cards

### Experience Page
- Timeline-style layout
- Skill tags with hover effects
- Detailed descriptions
- Visual card design

### Portfolio
- Project cards with descriptions
- Technology tags
- Links to resources
- Professional presentation

## 🎯 Before Your Interview

### High Priority Checklist
- [ ] Update email in `_config.yml`
- [ ] Replace profile picture
- [ ] Add AIDB paper details
- [ ] Fill in advisor name
- [ ] Update social media links
- [ ] Test all links work
- [ ] Deploy to BU server
- [ ] Test on mobile device

### Content Checklist
- [ ] About page complete
- [ ] Publications have descriptions
- [ ] Experience details filled in
- [ ] Portfolio projects described
- [ ] CV information complete
- [ ] News items accurate

## 🔧 Customization Tips

### Changing Colors
Edit `_sass/_base.scss`:
```scss
$theme-color: $dark_blue; // Change to any color
```

### Adding News Items
Edit `index.html`:
```html
<li class="news-item fade-in">
  <span class="news-date">Month Year</span>
  <span class="news-content">Your news here</span>
</li>
```

### Adding Publications
Edit `publications.md` and follow the template structure.

### Modifying Navigation
Edit `_includes/header.html` to add/remove menu items.

## 🐛 Troubleshooting

### Site not building?
- Check for syntax errors in YAML front matter
- Verify all HTML tags are closed
- Run `jekyll build` and read error messages

### Styles not applying?
- Clear browser cache
- Rebuild site: `bundle exec jekyll build`
- Check for typos in SCSS files

### Deployment issues?
- Verify SSH access to BU server
- Check file permissions
- Ensure correct directory path

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Font Awesome Icons](https://fontawesome.com/icons)
- [SCSS Guide](https://sass-lang.com/guide)

## 📄 License

This is your personal academic website. Customize it as needed!

## 🤝 Acknowledgments

Based on the *folio theme, significantly enhanced with:
- Modern animations and effects
- Professional academic layouts
- News highlights section
- Enhanced publications display
- Experience timeline
- CV page
- Mobile-responsive design

## 📧 Support

For questions about customization or deployment, refer to:
- QUICK_START.md for immediate help
- SETUP_INSTRUCTIONS.md for detailed guide
- CONTENT_EXAMPLES.md for content templates

---

**Good luck with your interview!** 🎓🚀

*Built with Jekyll • Designed for academics • Interview-ready*

Last updated: December 2025
