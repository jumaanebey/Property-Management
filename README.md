 # My Property Management Website

     A modern, responsive property management website built with Jekyll and
      deployed on GitHub Pages. Features include property listings with
     filtering, contact forms, and a complete property management service
     showcase.

     ## 🏠 Demo

     Visit the live website: [https://yourusername.github.io/my-property-ma
     nagement](https://yourusername.github.io/my-property-management)

     ## ✨ Features

     - **Responsive Design**: Mobile-first design that works on all devices
     - **Property Listings**: Dynamic property grid with advanced filtering
     - **Contact Forms**: Integrated contact forms with Formspree
     - **SEO Optimized**: Meta tags, structured data, and sitemap
     - **Accessibility**: WCAG 2.1 compliant with keyboard navigation
     - **Modern UI**: Tailwind CSS with custom property management theme
     - **Fast Loading**: Optimized images and lazy loading
     - **GitHub Pages Ready**: Automated deployment via GitHub Actions

     ## 🛠 Tech Stack

     - **Static Site Generator**: Jekyll 4.3
     - **CSS Framework**: Tailwind CSS 3.4
     - **Icons**: Font Awesome 6.4
     - **Fonts**: Google Fonts (Inter, Playfair Display)
     - **Forms**: Formspree integration
     - **Analytics**: Google Analytics 4 ready
     - **Deployment**: GitHub Pages with Actions
     - **Maps**: Google Maps embed

     ## 📁 Project Structure

     ```
     my-property-management/
     ├── _config.yml              # Jekyll configuration
     ├── _data/
     │   └── properties.yml       # Property data
     ├── _layouts/
     │   ├── default.html         # Base layout with navigation
     │   └── page.html            # Page layout with hero
     ├── _properties/             # Individual property pages
     ├── .github/workflows/
     │   └── deploy.yml           # GitHub Actions deployment
     ├── index.html               # Homepage
     ├── about.md                 # About page
     ├── services.md              # Services page
     ├── properties.html          # Properties listing with filters
     ├── contact.md               # Contact page with form
     ├── contact-thank-you.md     # Form submission thank you
     ├── robots.txt               # SEO robots file
     ├── Gemfile                  # Ruby dependencies
     └── README.md                # This file
     ```

     ## 🚀 Quick Start

     ### Prerequisites

     - Ruby 2.7+ (for local development)
     - Git
     - GitHub account

     ### Local Development

     1. **Clone the repository**
        ```bash
        git clone
     https://github.com/yourusername/my-property-management.git
        cd my-property-management
        ```

     2. **Install dependencies**
        ```bash
        bundle install
        ```

     3. **Serve locally**
        ```bash
        bundle exec jekyll serve
        ```

     4. **Open in browser**
        ```
        http://localhost:4000/my-property-management/
        ```

     ### GitHub Pages Deployment

     1. **Create a new repository** named `my-property-management` on
     GitHub
     2. **Push your code** to the `main` branch
     3. **Enable GitHub Pages**:
        - Go to repository Settings → Pages
        - Source: GitHub Actions
        - The site will auto-deploy via the included workflow

     ## 📝 Customization Guide

     ### 1. Basic Configuration

     Edit `_config.yml` to customize:

     ```yaml
     title: "Your Property Management Company"
     description: "Your company description"
     url: "https://yourusername.github.io"
     baseurl: "/your-repo-name"

     contact:
       phone: "Your phone number"
       email: "your@email.com"
       address: "Your business address"
     ```

     ### 2. Adding Properties

     Add new properties to `_data/properties.yml`:

     ```yaml
     - id: 9
       title: "Your Property Title"
       address: "Property Address"
       rent: 2500
       bedrooms: 2
       bathrooms: 2
       sqft: 1200
       city: "City Name"
       image: "https://your-image-url.jpg"
       slug: "property-url-slug"
       featured: true
       available: true
       description: "Property description"
       amenities:
         - "Amenity 1"
         - "Amenity 2"
     ```

     ### 3. Contact Form Setup

     1. **Sign up for Formspree**:
     [https://formspree.io](https://formspree.io)
     2. **Get your form endpoint**
     3. **Update `_config.yml`**:
        ```yaml
        formspree_endpoint: "https://formspree.io/f/your-form-id"
        ```

     ### 4. Google Analytics

     1. **Create GA4 property**
     2. **Update `_config.yml`**:
        ```yaml
        google_analytics: "G-XXXXXXXXXX"
        ```

     ### 5. Theme Colors

     Customize colors in `_layouts/default.html`:

     ```javascript
     tailwind.config = {
       theme: {
         extend: {
           colors: {
             primary: '#your-primary-color',
             secondary: '#your-secondary-color',
             accent: '#your-accent-color'
           }
         }
       }
     }
     ```

     ## 🏡 Property Management

     ### Adding New Properties

     1. **Update data file**: Add property details to 
     `_data/properties.yml`
     2. **Add images**: Use high-quality images (recommended: Unsplash)
     3. **SEO optimization**: Include descriptive titles and descriptions

     ### Property Images

     **Recommended specifications**:
     - **Thumbnail**: 400×300px
     - **Gallery**: 800×600px
     - **Format**: JPG for photos, PNG for graphics
     - **Quality**: 70-80% for web optimization

     **Image sources**:
     - [Unsplash](https://unsplash.com) - Free high-quality photos
     - [Pexels](https://pexels.com) - Free stock photos
     - Professional photography for actual properties

     ### Property Filtering

     The site includes JavaScript-powered filtering by:
     - City/Location
     - Number of bedrooms
     - Maximum rent price
     - Availability status

     ## 🎨 Design System

     ### Typography
     - **Headings**: Playfair Display (serif)
     - **Body**: Inter (sans-serif)
     - **Scale**: Tailwind's default type scale

     ### Colors
     - **Primary**: Blue (#1e40af)
     - **Secondary**: Light Blue (#3b82f6)
     - **Accent**: Amber (#f59e0b)
     - **Success**: Emerald (#10b981)
     - **Error**: Red (#ef4444)

     ### Components
     - **Cards**: Rounded corners, subtle shadows
     - **Buttons**: Rounded pills for primary actions
     - **Forms**: Clean inputs with focus states
     - **Navigation**: Fixed header with mobile menu

     ## ♿ Accessibility

     The site follows WCAG 2.1 guidelines:

     - **Keyboard Navigation**: All interactive elements accessible via 
     keyboard
     - **Screen Reader Support**: Proper ARIA labels and semantic HTML
     - **Color Contrast**: AA compliant contrast ratios
     - **Focus Management**: Visible focus indicators
     - **Alt Text**: Descriptive alt text for all images

     ### Accessibility Checklist

     - [ ] Test with keyboard navigation
     - [ ] Verify with screen reader (NVDA/JAWS)
     - [ ] Check color contrast ratios
     - [ ] Validate HTML structure
     - [ ] Test form error states

     ## 🚀 Performance

     ### Optimization Features

     - **Lazy Loading**: Images load as needed
     - **CDN Assets**: Tailwind and Font Awesome via CDN
     - **Minified CSS**: Compressed in production
     - **Optimized Images**: WebP format when possible
     - **Caching**: Browser caching headers

     ### Performance Tips

     1. **Optimize Images**:
        ```bash
        # Use tools like ImageOptim or TinyPNG
        # Convert to WebP when possible
        # Implement responsive images
        ```

     2. **Monitor Performance**:
        - Use Google PageSpeed Insights
        - Test on various devices
        - Monitor Core Web Vitals

     ## 🔧 Troubleshooting

     ### Common Issues

     **Jekyll build fails**:
     ```bash
     # Clear cache and rebuild
     bundle exec jekyll clean
     bundle exec jekyll build
     ```

     **GitHub Pages not updating**:
     - Check Actions tab for build errors
     - Verify branch settings in repository
     - Ensure `_config.yml` has correct baseurl

     **Forms not working**:
     - Verify Formspree endpoint URL
     - Check form action and method
     - Test form submission manually

     **Images not loading**:
     - Verify image URLs are accessible
     - Check for HTTPS vs HTTP issues
     - Ensure proper alt text

     ### Development Tips

     1. **Local Testing**:
        ```bash
        # Test with production settings
        JEKYLL_ENV=production bundle exec jekyll serve
        ```

     2. **Debugging**:
        ```bash
        # Verbose output
        bundle exec jekyll serve --verbose
        ```

     3. **Live Reload**:
        ```bash
        # Auto-refresh on changes
        bundle exec jekyll serve --livereload
        ```

     ## 📱 Mobile Responsiveness

     The site is fully responsive with breakpoints:

     - **Mobile**: < 768px
     - **Tablet**: 768px - 1024px
     - **Desktop**: > 1024px

     ### Testing Checklist

     - [ ] Navigation menu on mobile
     - [ ] Property cards layout
     - [ ] Contact form usability
     - [ ] Image scaling
     - [ ] Touch targets (minimum 44px)

     ## 🤝 Contributing

     1. Fork the repository
     2. Create a feature branch
     3. Make your changes
     4. Test thoroughly
     5. Submit a pull request

     ### Development Guidelines

     - Use semantic HTML
     - Follow existing code style
     - Test on multiple devices
     - Optimize for performance
     - Maintain accessibility standards

     ## 📄 License

     This project is licensed under the MIT License - see the 
     [LICENSE](LICENSE) file for details.

     ## 🆘 Support

     - **Documentation**: This README
     - **Issues**: [GitHub 
     Issues](https://github.com/yourusername/my-property-management/issues)
     - **Discussions**: [GitHub Discussions](https://github.com/yourusernam
     e/my-property-management/discussions)

     ## 🚀 Deployment Steps

     ### Ready to go live? Follow these steps:

     1. **Customize Configuration**
        - Update `_config.yml` with your information
        - Replace placeholder content with your actual data
        - Set up Formspree for contact forms

     2. **Update Content**
        - Replace sample properties with real listings
        - Add your team information to About page
        - Customize service descriptions

     3. **Set Up Integrations**
        - Configure Google Analytics
        - Set up Formspree contact forms
        - Add Google Maps API key if needed

     4. **Deploy to GitHub Pages**
        - Push to `main` branch
        - Enable GitHub Pages with Actions
        - Your site will be live at 
     `https://yourusername.github.io/my-property-management`

     5. **Custom Domain (Optional)**
        - Purchase domain name
        - Configure DNS settings
        - Update GitHub Pages settings

     ---

     **Happy property managing! 🏠**
