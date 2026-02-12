# Finn Plumbing & Heating Website

Professional service-based website for plumbing and heating services, focusing on oil boiler work and bathroom installation.

## Features

- ✅ SEO-optimized landing page with hero section, service cards, gallery, about section, FAQ accordion
- ✅ Separate booking page with date/time picker form that opens email client
- ✅ Responsive mobile-first design
- ✅ Google Analytics 4 integration with event tracking
- ✅ Structured data (JSON-LD) for LocalBusiness, Service, FAQPage
- ✅ Complete meta tags (title, description, Open Graph, Twitter Cards, canonical URLs)
- ✅ robots.txt and sitemap.xml files

## File Structure

```
/
├── index.html          # Main landing page
├── booking.html        # Booking page with form
├── styles.css          # All styles (mobile-first responsive)
├── script.js           # JavaScript for interactivity and GA4 tracking
├── robots.txt          # Search engine crawler instructions
├── sitemap.xml         # XML sitemap for SEO
└── assets/
    ├── work1.jpg       # Gallery image 1
    ├── work2.jpg       # Gallery image 2
    ├── work3.jpg       # Gallery image 3
    ├── work4.jpg       # Gallery image 4
    ├── work5.jpg       # Gallery image 5
    └── work6.jpg       # Gallery image 6
```

## Setup Instructions

### 1. Add Your Images
Place your 6 gallery images in the `assets/` folder:
- `work1.jpg` through `work6.jpg`

### 2. Update Company Information
Edit the following files to add your specific details:

**index.html:**
- Replace `G-XXXXXXXXXX` with your Google Analytics 4 Measurement ID
- Update phone number: `+44-XXXX-XXXXXX`
- Update email: `info@finnplumbingheating.co.uk`
- Update company name if different from "Finn Plumbing & Heating"
- Update structured data with your actual business address and coordinates

**booking.html:**
- Replace `G-XXXXXXXXXX` with your Google Analytics 4 Measurement ID
- Update email in the form handler: `info@finnplumbingheating.co.uk`

### 3. Update URLs
Replace `https://www.finnplumbingheating.co.uk` with your actual domain in:
- `index.html` (Open Graph, Twitter Cards, canonical URLs, structured data)
- `booking.html` (Open Graph, Twitter Cards, canonical URLs)
- `sitemap.xml` (all URLs)
- `robots.txt` (sitemap URL)

### 4. Google Analytics Setup
1. Create a Google Analytics 4 property
2. Get your Measurement ID (format: G-XXXXXXXXXX)
3. Replace `G-XXXXXXXXXX` in both HTML files
4. Event tracking is already implemented for:
   - CTA button clicks
   - Form submissions
   - FAQ interactions
   - Navigation clicks
   - Mobile menu toggles

### 5. Brand Colors (Current)
The website uses a professional blue and orange color scheme:
- Primary Blue: `#0066CC`
- Secondary Orange: `#FF6600`

To change colors, edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #0066CC;
    --secondary-color: #FF6600;
    /* ... */
}
```

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Responsive design works on all screen sizes

## SEO Features

- Semantic HTML5 structure
- Meta tags (title, description, keywords)
- Open Graph tags for social sharing
- Twitter Card tags
- Canonical URLs
- Structured data (JSON-LD) for:
  - LocalBusiness
  - Service
  - FAQPage
- robots.txt for search engine crawlers
- XML sitemap
- Alt text on images
- Proper heading hierarchy

## Contact Form

The booking form opens the user's default email client with pre-filled information. Make sure to:
1. Update the email address in `script.js` (line with `mailto:`)
2. Test the form to ensure emails are formatted correctly

## Testing Checklist

- [ ] All images load correctly
- [ ] Mobile menu works on mobile devices
- [ ] FAQ accordion expands/collapses properly
- [ ] Booking form opens email client correctly
- [ ] All links work
- [ ] Google Analytics tracking works
- [ ] Responsive design works on all screen sizes
- [ ] Form validation works
- [ ] Smooth scrolling works for anchor links

## Notes

- The website uses vanilla JavaScript (no frameworks)
- All CSS is mobile-first responsive
- The design is modern and professional
- Service area postcodes are listed in the about section
- The booking form uses `mailto:` to open email client (no backend required)
