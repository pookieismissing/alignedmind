# Aligned Mind Psychology and Wellness - Website

A professional, multi-page website for your psychology practice built with HTML, CSS, and JavaScript.

## 📁 Website Structure

```
aligned-mind-website/
├── index.html           # Home page
├── about.html           # About page
├── services.html        # Services page
├── contact.html         # Contact page
├── faq.html            # FAQ page
├── practice-info.html  # Practice information (policies, payment, privacy, terms)
├── styles.css          # All styling
├── script.js           # Interactive functionality
├── README.md           # This file
└── DEPLOYMENT.md       # GitHub Pages deployment guide
```

## 🎨 Design Features

- **Color Scheme**: Dark grey/black (#1a1a1a, #2d2d2d) with sage green accents (#8b9d83)
- **Typography**: Crimson Pro (serif) for headings, Montserrat (sans-serif) for body text
- **Aesthetic**: Refined, calming, professional with smooth animations
- **Responsive**: Fully mobile-friendly design
- **Multi-page**: Separate pages for easy navigation and SEO

## 📄 Pages Overview

### 1. Home (index.html)
- Hero section with tagline
- Quick info cards (location, contact, hours)
- Services preview
- Call-to-action section

### 2. About (about.html)
- Practice philosophy
- Meet Ann section
- Core values
- Therapeutic approach

### 3. Services (services.html)
- Depression treatment details
- Anxiety management details
- Trauma therapy details
- Treatment approach explanation
- Session options (in-person/telehealth)

### 4. Contact (contact.html)
- Contact form
- Location and hours
- Phone, email, social media
- Map placeholder
- Emergency information

### 5. FAQ (faq.html)
- Interactive accordion with 12 common questions
- Topics: getting started, insurance, confidentiality, session details

### 6. Practice Information (practice-info.html)
- Tabbed interface with 4 sections:
  - Practice Policies
  - Payment & Insurance
  - Privacy Policy (HIPAA)
  - Terms of Service

## 🚀 Quick Start

### Local Testing
1. Download all files to the same folder
2. Double-click `index.html` to open in your browser
3. Navigate between pages using the menu

### Deploy to GitHub Pages
See **DEPLOYMENT.md** for detailed instructions on deploying to GitHub Pages for free hosting and testing.

## ✏️ Customization Guide

### Update Contact Information
All pages already include your contact info:
- **Address**: 44 River Street, Suite 1A, Milford, CT 06460
- **Phone**: (203) 293-2575
- **Email**: ann@alignedmindpsychiatryandwellness.com
- **Instagram**: @alignedmindpsych

### Update Patient Portal Link
Replace `https://portal.example.com` in all HTML files with your actual portal URL. Files to update:
- index.html
- about.html
- services.html
- contact.html
- faq.html
- practice-info.html

### Add Your Logo
Replace the text logo in the navigation with an image. Update in all HTML files:
```html
<!-- Replace this: -->
<a href="index.html" class="logo">
    <span class="logo-main">Aligned Mind</span>
    <span class="logo-sub">Psychology & Wellness</span>
</a>

<!-- With this: -->
<a href="index.html" class="logo">
    <img src="logo.png" alt="Aligned Mind Logo" style="height: 50px;">
</a>
```

### Add Professional Photo
In `about.html`, replace the placeholder:
```html
<div class="image-placeholder">
    <!-- Replace this entire div with: -->
    <img src="headshot.jpg" alt="Ann - Therapist" style="width: 100%; border-radius: 8px;">
</div>
```

### Add Google Map
In `contact.html`, replace the map placeholder:
1. Go to Google Maps
2. Search for "44 River Street, Milford, CT"
3. Click "Share" → "Embed a map"
4. Copy the iframe code
5. Replace the map-placeholder div with the iframe

### Connect Contact Form
The contact form currently shows an alert. To make it functional:

**Option 1: Formspree (Easiest)**
1. Sign up at https://formspree.io
2. Create a new form
3. Update `contact.html`:
```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option 2: Netlify Forms (if hosting on Netlify)**
1. Add `netlify` attribute to form:
```html
<form class="contact-form" name="contact" method="POST" data-netlify="true">
```

**Option 3: EmailJS**
1. Sign up at https://www.emailjs.com
2. Follow their documentation to add the SDK
3. Update the JavaScript in `script.js`

### Customize Colors
Update the CSS variables in `styles.css`:
```css
:root {
    --color-dark: #1a1a1a;          /* Main dark color */
    --color-charcoal: #2d2d2d;      /* Secondary dark */
    --color-sage: #8b9d83;          /* Accent color */
    --color-sage-light: #a8b9a0;    /* Light accent */
    /* etc. */
}
```

### Add More Services
In `services.html`, duplicate a service card:
```html
<div class="service-card">
    <div class="service-icon">
        <!-- SVG icon -->
    </div>
    <h3>New Service Name</h3>
    <p>Description...</p>
    <ul class="service-features">
        <li>Feature 1</li>
        <li>Feature 2</li>
    </ul>
</div>
```

## 🌟 Features Included

✅ Multi-page structure for better SEO
✅ Smooth scrolling navigation
✅ Mobile-responsive hamburger menu
✅ Interactive FAQ accordion
✅ Tabbed Practice Information section
✅ Contact form with validation
✅ Scroll animations
✅ Sticky navigation bar
✅ Page-specific active nav highlighting
✅ Accessibility features (keyboard navigation, ARIA labels)

## 📱 Responsive Breakpoints

- **Desktop**: 1024px and above
- **Tablet**: 768px - 1023px
- **Mobile**: 767px and below

## 🔧 Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📋 Pre-Launch Checklist

Before going live:

### Content
- [ ] Add professional headshot photo
- [ ] Add logo to navigation
- [ ] Review and customize all page content
- [ ] Add actual office photos (optional)
- [ ] Update hours if different
- [ ] Verify all contact information

### Functionality
- [ ] Update patient portal URL
- [ ] Connect contact form
- [ ] Add Google Maps embed
- [ ] Test all navigation links
- [ ] Test FAQ accordion
- [ ] Test Practice Info tabs
- [ ] Test mobile menu

### SEO & Meta
- [ ] Add meta descriptions to all pages
- [ ] Add Open Graph tags for social sharing
- [ ] Create favicon
- [ ] Submit sitemap to Google

### Legal & Compliance
- [ ] Ensure HIPAA compliance for forms
- [ ] Review privacy policy with legal counsel
- [ ] Add SSL certificate (HTTPS)
- [ ] Cookie consent if needed

## 💡 Recommended Next Steps

1. **Deploy to GitHub Pages** - See DEPLOYMENT.md for instructions
2. **Test thoroughly** - Check on multiple devices and browsers
3. **Get SSL certificate** - GitHub Pages provides this automatically
4. **Set up analytics** - Add Google Analytics or similar
5. **Submit to search engines** - Google Search Console, Bing Webmaster
6. **Get a custom domain** - More professional than github.io URL
7. **Add schema markup** - For better SEO
8. **Set up online booking** - Integrate scheduling system

## 🔒 HIPAA Compliance Notes

When going live:
- Ensure contact forms use encrypted connections (HTTPS)
- Patient portal must be HIPAA-compliant
- Do not collect PHI (Protected Health Information) on public forms
- Privacy policy should be comprehensive and reviewed by legal
- Any analytics tools must be HIPAA-compliant or configured properly
- Consider Business Associate Agreements for third-party services

## 🎨 Advanced Customization

### Adding a Blog
1. Create a `blog` folder
2. Create individual blog post HTML files
3. Create a blog listing page
4. Update navigation to include blog link

### Adding Testimonials
Add a testimonials section to index.html or about.html:
```html
<section class="testimonials">
    <div class="container">
        <div class="section-header">
            <h2 class="section-title">Client Testimonials</h2>
            <div class="title-accent"></div>
        </div>
        <div class="testimonial-grid">
            <!-- Add testimonial cards -->
        </div>
    </div>
</section>
```

### Adding Team Members
If you expand, add team member profiles in about.html

### Multilingual Support
For Spanish or other language support, create duplicate pages with language suffix (e.g., `index-es.html`)

## 📞 Support & Questions

If you need help customizing the website:
1. Check this README
2. Review DEPLOYMENT.md for GitHub Pages help
3. Inspect the code comments for guidance
4. Test changes in local browser before deploying

## 📄 License

This website template is provided for Aligned Mind Psychology and Wellness. Feel free to customize as needed for your practice.

---

**Built with care for Aligned Mind Psychology and Wellness**  
*Where mental health meets inner balance*
