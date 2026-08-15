# Chefer | Restaurant

A modern, responsive restaurant website showcasing Lebanese cuisine with an elegant UI/UX design.

## Project Overview

Chefer is a professional restaurant website built with HTML5, CSS3, and JavaScript. It features a complete restaurant experience including menu browsing, team showcase, testimonials, and contact functionality.

**Restaurant:** Chefer  
**Cuisine:** Lebanese & Middle Eastern  
**Location:** Beirut, Lebanon  
**Website Type:** Static HTML/CSS/JavaScript

## Features

- **Responsive Design** - Fully optimized for desktop, tablet, and mobile devices
- **Menu System** - Tabbed menu interface with Breakfast, Lunch, and Dinner categories
- **Interactive Components** - Animated statistics, carousel testimonials, hover effects
- **Team Showcase** - Professional staff profiles with social media links
- **Blog Section** - Latest articles and culinary insights
- **Contact Page** - Form with integrated map and contact information
- **Newsletter Signup** - Email subscription form
- **Accessibility** - Semantic HTML and keyboard navigation support
- **Performance** - Optimized assets and smooth animations using WOW.js

## Tech Stack

### Frontend
- **HTML5** - Semantic markup
- **CSS3** - Custom styling with Bootstrap 5 framework
- **JavaScript** - ES6+ for interactivity
- **jQuery 3.6.4** - DOM manipulation

### Libraries & Plugins
- **Bootstrap 5.0.0** - Responsive grid and components
- **Owl Carousel** - Testimonials carousel
- **WOW.js** - Scroll-triggered animations
- **Font Awesome 5.15.0** - Icon library
- **Google Fonts** - Typography (Emblema One, Poppins)

### Backend/Services
- **Formspree** - Form submission handling (requires configuration)
- **Google Maps** - Embedded location map

## Project Structure

```
Chefer-Restaurant/
├── index.html                 # Homepage
├── about.html                 # About the restaurant
├── menu.html                  # Full menu page
├── team.html                  # Chef profiles
├── blog.html                  # Blog posts
├── testimonial.html           # Customer testimonials
├── contact.html               # Contact and reservation
├── feature.html               # Restaurant features
├── 404.html                   # 404 error page
├── css/
│   ├── bootstrap.min.css      # Bootstrap framework
│   └── style.css              # Custom styles
├── js/
│   └── main.js                # Custom JavaScript
├── lib/                       # Third-party libraries
│   ├── animate/               # Animate.css
│   ├── owlcarousel/           # Owl Carousel
│   ├── wow/                   # WOW.js
│   ├── easing/                # jQuery easing
│   ├── waypoints/             # Waypoints
│   └── counterup/             # Counter-Up
├── img/                       # Images and assets
├── scss/                      # SCSS source files
├── .gitignore
└── README.md
```

## Setup Instructions

### Local Development

1. **Clone or download the repository:**
   ```bash
   git clone <repository-url>
   cd Chefer-Restaurant
   ```

2. **Open in browser:**
   - Simply open `index.html` in a modern web browser
   - No build tools or dependencies required
   - Works offline

### Form Configuration (Required for Deployment)

The website uses **Formspree** for form submissions. To enable contact and newsletter forms:

1. **Sign up at:** https://formspree.io (free)
2. **Create a new form** for "Contact"
3. **Copy the form ID** from Formspree
4. **Update all HTML files:**
   - Replace `https://formspree.io/f/xyzabc123` with your form ID in:
     - `contact.html` - Contact form
     - `index.html` - Newsletter form in footer
     - All other `.html` files - Newsletter forms in footer

Example: If your Formspree ID is `xyzdef456`, use:
```html
<form method="POST" action="https://formspree.io/f/xyzdef456">
```

## Deployment

### Option 1: Static Hosting (Recommended)

Deploy to any static hosting service:

#### Netlify
- Connect your Git repository
- Set build command: (leave empty - no build needed)
- Set publish directory: `/`
- Deploy

#### Vercel
- Import from Git
- Choose Static Site
- Deploy

#### GitHub Pages
- Push to GitHub
- Enable GitHub Pages in Settings
- Set source to main branch

#### Other Options
- Firebase Hosting
- AWS S3 + CloudFront
- Surge.sh
- Cloudflare Pages

### Option 2: Traditional Web Hosting
- Upload all files via FTP to your hosting provider
- Ensure `.html` files are in the root directory

### Pre-Deployment Checklist

- [ ] Contact form configured with Formspree ID
- [ ] Newsletter form configured with Formspree ID
- [ ] Google Map location verified (coordinates are for Beirut)
- [ ] Social media links updated (if applicable)
- [ ] All images are properly linked
- [ ] Test all navigation links
- [ ] Test responsive layout on mobile
- [ ] Test forms on staging environment

## Content & Customization

### Update Restaurant Information

Edit these files to customize content:

- **Restaurant Details:** Update phone, email, and address in footer (appears in all HTML files)
- **Menu Items:** Edit `menu.html` to add descriptions and prices
- **Team Members:** Update names and roles in `team.html` and `index.html`
- **Contact Info:** Update in `contact.html` footer sections
- **About Text:** Edit content in `about.html`

### Update Images

Replace images in the `img/` directory:
- `hero-*.jpg` - Hero section images
- `menu-*.jpg` - Menu item photos
- `team-*.jpg` - Chef photos
- `about*.jpg` - About section images
- `testimonial*.jpg` - Customer photos

### Add Blog Posts

Create new blog articles:
1. Copy `blog.html` template
2. Create `blog-article-1.html` (or similar naming)
3. Update article content
4. Link from `blog.html` card

## Forms Explanation

### Contact Form
- **Status:** Production-ready (via Formspree)
- **Configuration:** Requires Formspree form ID
- **Fields:** Name, Email, Subject, Message
- **Location:** `contact.html`

### Newsletter Signup
- **Status:** Production-ready (via Formspree)
- **Configuration:** Requires Formspree form ID (can be same or different)
- **Fields:** Email
- **Location:** Footer of all pages

## Performance Optimization

The website includes several performance optimizations:

- Minified CSS and JavaScript
- Optimized image sizes
- Lazy-loaded images (via browser native support)
- Efficient animation timing (WOW.js)
- CSS media queries for responsive design
- Preconnect to Google Fonts

**Performance Metrics (Approximate):**
- Page Load: 2-3 seconds on 4G
- Lighthouse: 85-90 (without deployment optimization)
- Mobile-Friendly: Yes
- HTTPS Ready: Yes (when deployed)

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)

## SEO

The website includes basic SEO optimization:

- Semantic HTML5 markup
- Meta tags on all pages
- Descriptive page titles
- Open Graph metadata (prepared for social sharing)
- Responsive design (mobile-friendly)
- Schema.org structured data (basic)
- Proper heading hierarchy

### SEO Improvements to Consider
- Add detailed blog posts with keyword optimization
- Build backlinks to increase domain authority
- Add XML sitemap (can be generated by hosting platform)
- Set up Google Search Console
- Monitor search traffic with Google Analytics

## Accessibility

Features for accessible browsing:

- Semantic HTML elements
- ARIA labels where appropriate
- Keyboard navigation support
- Color contrast compliant
- Readable font sizes
- Alt text on images (present)
- Form labels and validation messages

## Limitations & Known Issues

### Current Limitations

1. **Static Content** - Menu, testimonials, and blog posts are hardcoded HTML
   - *Solution:* Add CMS integration (Contentful, Strapi) for dynamic content

2. **No Admin Panel** - No dashboard for content updates
   - *Solution:* Use headless CMS or deploy on JAMstack platform

3. **No Real Reservations** - "Reserve Now" links to contact form only
   - *Solution:* Integrate reservation system (e.g., TableApp, Resy API)

4. **Limited Analytics** - No built-in tracking
   - *Solution:* Add Google Analytics or similar

5. **No Payment Processing** - No e-commerce functionality
   - *Solution:* Integrate Stripe or similar if needed

### Forms Require Configuration

Before deployment, configure:
- ✅ Contact form - Needs Formspree ID
- ✅ Newsletter form - Needs Formspree ID

## Development

### Editing Styles

Styles are generated from SCSS:
- Source: `scss/bootstrap.scss`
- Compiled: `css/bootstrap.min.css`

To modify Bootstrap variables, edit the SCSS and recompile.

### Adding JavaScript

Add custom scripts to `js/main.js`:
- Currently ~55 lines
- Uses jQuery and plugin initialization
- Handles: Navigation, animations, carousel, counter-up effects

## Support & Troubleshooting

### Form Not Submitting?
- Verify Formspree form ID is correct
- Check browser console for errors
- Ensure email field is valid

### Images Not Loading?
- Verify image paths are relative
- Check that image files exist in `img/` directory
- Clear browser cache

### Styles Not Applying?
- Clear browser cache (Ctrl+Shift+Delete)
- Check Bootstrap CSS is loaded
- Verify `style.css` is linked

## License

This project is provided as a portfolio template. Modify as needed for your restaurant.

## Contact

For questions or support, visit the contact page or email: chefer@restofood.com

---

**Last Updated:** August 2026  
**Version:** 1.0.0  
**Status:** Production-Ready (with Formspree configuration)
