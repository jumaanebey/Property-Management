  ---
  layout: page
  title: "Contact Us"
  subtitle: "Get in touch for your property management needs"
  description: "Contact My Property Management for professional property
  management services. Schedule a consultation, ask questions, or get
  started today."
  ---

  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-12">

  <!-- Contact Form -->
  <div class="bg-white rounded-lg shadow-lg p-8">
    <h3 class="text-2xl font-bold text-gray-900 mb-6">Send Us a
  Message</h3>

    <form action="{{ site.formspree_endpoint }}" method="POST" 
  class="space-y-6" id="contact-form">
      <input type="hidden" name="_subject" value="Website Contact Form
  Submission">
      <input type="hidden" name="_next" value="{{ '/contact-thank-you/' |
  absolute_url }}">

      <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div>
          <label for="first-name" class="block text-sm font-medium
  text-gray-700 mb-2">First Name *</label>
          <input
            type="text"
            id="first-name"
            name="first-name"
            required
            class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
            placeholder="John"
          >
        </div>

        <div>
          <label for="last-name" class="block text-sm font-medium
  text-gray-700 mb-2">Last Name *</label>
          <input
            type="text"
            id="last-name"
            name="last-name"
            required
            class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
            placeholder="Smith"
          >
        </div>
      </div>

      <div>
        <label for="email" class="block text-sm font-medium text-gray-700
  mb-2">Email Address *</label>
        <input
          type="email"
          id="email"
          name="email"
          required
          class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
          placeholder="john.smith@email.com"
        >
      </div>

      <div>
        <label for="phone" class="block text-sm font-medium text-gray-700
  mb-2">Phone Number</label>
        <input
          type="tel"
          id="phone"
          name="phone"
          class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
          placeholder="(555) 123-4567"
        >
      </div>

      <div>
        <label for="property-address" class="block text-sm font-medium
  text-gray-700 mb-2">Property Address (if applicable)</label>
        <input
          type="text"
          id="property-address"
          name="property-address"
          class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
          placeholder="123 Main Street, City, State 12345"
        >
      </div>

      <div>
        <label for="inquiry-type" class="block text-sm font-medium
  text-gray-700 mb-2">Type of Inquiry *</label>
        <select
          id="inquiry-type"
          name="inquiry-type"
          required
          class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
        >
          <option value="">Please select...</option>
          <option value="property-management">Property Management
  Services</option>
          <option value="tenant-inquiry">I'm Looking to Rent</option>
          <option value="property-rental">Rent My Property</option>
          <option value="consultation">Free Consultation</option>
          <option value="maintenance">Maintenance Request</option>
          <option value="general">General Question</option>
          <option value="other">Other</option>
        </select>
      </div>

      <div>
        <label for="message" class="block text-sm font-medium
  text-gray-700 mb-2">Message *</label>
        <textarea
          id="message"
          name="message"
          rows="5"
          required
          class="w-full px-4 py-3 border border-gray-300 rounded-md
  focus:outline-none focus:ring-2 focus:ring-primary
  focus:border-transparent"
          placeholder="Please tell us about your property management needs
   or any questions you have..."
        ></textarea>
      </div>

      <div class="flex items-start">
        <input
          type="checkbox"
          id="newsletter"
          name="newsletter"
          value="yes"
          class="mt-1 h-4 w-4 text-primary focus:ring-primary
  border-gray-300 rounded"
        >
        <label for="newsletter" class="ml-2 text-sm text-gray-600">
          I'd like to receive occasional updates about property management
   tips and market insights.
        </label>
      </div>

      <button
        type="submit"
        class="w-full bg-primary text-white py-3 px-6 rounded-md
  hover:bg-blue-700 transition-colors font-medium text-lg focus-ring"
      >
        <i class="fas fa-paper-plane mr-2"></i>
        Send Message
      </button>

      <p class="text-sm text-gray-500 text-center">
        We typically respond within 2-4 hours during business days.
      </p>
    </form>
  </div>

  <!-- Contact Information -->
  <div class="space-y-8">

    <!-- Contact Details -->
    <div class="bg-primary text-white rounded-lg p-8">
      <h3 class="text-2xl font-bold mb-6">Get in Touch</h3>

      <div class="space-y-4">
        <div class="flex items-start">
          <i class="fas fa-map-marker-alt text-accent text-xl mt-1
  mr-4"></i>
          <div>
            <h4 class="font-semibold mb-1">Our Office</h4>
            <p class="text-blue-100">{{ site.contact.address }}</p>
          </div>
        </div>

        <div class="flex items-start">
          <i class="fas fa-phone text-accent text-xl mt-1 mr-4"></i>
          <div>
            <h4 class="font-semibold mb-1">Phone</h4>
            <a href="tel:{{ site.contact.phone }}" class="text-blue-100
  hover:text-white transition-colors">
              {{ site.contact.phone }}
            </a>
            <p class="text-sm text-blue-200">24/7 Emergency Line
  Available</p>
          </div>
        </div>

        <div class="flex items-start">
          <i class="fas fa-envelope text-accent text-xl mt-1 mr-4"></i>
          <div>
            <h4 class="font-semibold mb-1">Email</h4>
            <a href="mailto:{{ site.contact.email }}" class="text-blue-100
   hover:text-white transition-colors">
              {{ site.contact.email }}
            </a>
            <p class="text-sm text-blue-200">We respond within 2-4
  hours</p>
          </div>
        </div>

        <div class="flex items-start">
          <i class="fas fa-clock text-accent text-xl mt-1 mr-4"></i>
          <div>
            <h4 class="font-semibold mb-1">Business Hours</h4>
            <div class="text-blue-100 text-sm space-y-1">
              <p>Monday - Friday: 8:00 AM - 6:00 PM</p>
              <p>Saturday: 9:00 AM - 4:00 PM</p>
              <p>Sunday: Emergency calls only</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Quick Actions -->
    <div class="bg-gray-50 rounded-lg p-6">
      <h4 class="text-xl font-bold text-gray-900 mb-4">Quick Actions</h4>
      <div class="space-y-3">
        <a
          href="tel:{{ site.contact.phone }}"
          class="flex items-center justify-between p-3 bg-white rounded-lg
   border border-gray-200 hover:border-primary transition-colors group
  focus-ring"
        >
          <div class="flex items-center">
            <i class="fas fa-phone text-primary mr-3"></i>
            <span class="font-medium">Call Now</span>
          </div>
          <i class="fas fa-arrow-right text-gray-400
  group-hover:text-primary transition-colors"></i>
        </a>

        <a
          href="mailto:{{ site.contact.email }}"
          class="flex items-center justify-between p-3 bg-white rounded-lg
   border border-gray-200 hover:border-primary transition-colors group
  focus-ring"
        >
          <div class="flex items-center">
            <i class="fas fa-envelope text-primary mr-3"></i>
            <span class="font-medium">Send Email</span>
          </div>
          <i class="fas fa-arrow-right text-gray-400
  group-hover:text-primary transition-colors"></i>
        </a>

        <a
          href="{{ '/properties/' | relative_url }}"
          class="flex items-center justify-between p-3 bg-white rounded-lg
   border border-gray-200 hover:border-primary transition-colors group
  focus-ring"
        >
          <div class="flex items-center">
            <i class="fas fa-home text-primary mr-3"></i>
            <span class="font-medium">View Properties</span>
          </div>
          <i class="fas fa-arrow-right text-gray-400
  group-hover:text-primary transition-colors"></i>
        </a>
      </div>
    </div>

    <!-- Emergency Contact -->
    <div class="bg-red-50 border border-red-200 rounded-lg p-6">
      <h4 class="text-lg font-bold text-red-800 mb-2">
        <i class="fas fa-exclamation-triangle mr-2"></i>
        Emergency Maintenance
      </h4>
      <p class="text-red-700 text-sm mb-3">
        For urgent maintenance issues (water leaks, electrical problems,
  security concerns), call our 24/7 emergency line:
      </p>
      <a
        href="tel:+1-555-363-7436"
        class="text-lg font-bold text-red-800 hover:text-red-900
  focus-ring"
      >
        (555) 363-7436
      </a>
    </div>

  </div>

  </div>

  <!-- Map Section -->
  <div class="mb-12">
    <h3 class="text-2xl font-bold text-gray-900 mb-6 text-center">Visit
  Our Office</h3>
    <div class="bg-gray-200 rounded-lg overflow-hidden shadow-lg" 
  style="height: 400px;">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3024.12
  34567890123!2d-74.0059728!3d40.7484405!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!
  4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDDCsDQ0JzU0LjQiTiA3NMKwMDAnMjEuNSJX!5e0!3m
  2!1sen!2sus!4v1234567890123!5m2!1sen!2sus"
        width="100%"
        height="400"
        style="border:0;"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
        title="My Property Management Office Location"
      ></iframe>
    </div>
    <div class="mt-4 text-center">
      <p class="text-gray-600">
        <i class="fas fa-map-marker-alt text-primary mr-2"></i>
        {{ site.contact.address }}
      </p>
      <p class="text-sm text-gray-500 mt-2">
        Free parking available | Wheelchair accessible | Public transit
  nearby
      </p>
    </div>
  </div>

  <!-- FAQ Section -->
  <div class="bg-gray-50 rounded-lg p-8">
    <h3 class="text-2xl font-bold text-gray-900 mb-6 
  text-center">Frequently Asked Questions</h3>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div>
        <h4 class="font-bold text-gray-900 mb-2">How quickly do you
  respond to inquiries?</h4>
        <p class="text-gray-600 text-sm">We typically respond to all
  inquiries within 2-4 hours during business days, and within 24 hours on
  weekends.</p>
      </div>

      <div>
        <h4 class="font-bold text-gray-900 mb-2">Do you offer free
  consultations?</h4>
        <p class="text-gray-600 text-sm">Yes! We provide free,
  no-obligation consultations for all property owners interested in our
  management services.</p>
      </div>

      <div>
        <h4 class="font-bold text-gray-900 mb-2">What areas do you
  serve?</h4>
        <p class="text-gray-600 text-sm">We serve the entire metropolitan
  area including downtown, suburban, and surrounding communities within a
  25-mile radius.</p>
      </div>

      <div>
        <h4 class="font-bold text-gray-900 mb-2">How do I schedule a
  property viewing?</h4>
        <p class="text-gray-600 text-sm">You can call us directly, use the
   contact form above, or click "Contact" on any property listing to
  schedule a viewing.</p>
      </div>
    </div>
  </div>

  <script>
  document.addEventListener('DOMContentLoaded', function() {
    // Pre-fill property field if coming from property page
    const urlParams = new URLSearchParams(window.location.search);
    const propertyParam = urlParams.get('property');
    if (propertyParam) {
      document.getElementById('property-address').value = propertyParam;
      document.getElementById('inquiry-type').value = 'tenant-inquiry';

      // Scroll to form
      document.getElementById('contact-form').scrollIntoView({
        behavior: 'smooth',
        block: 'start'
      });
    }

    // Form submission handling
    const form = document.getElementById('contact-form');
    form.addEventListener('submit', function(e) {
      // You can add custom validation or tracking here
      console.log('Contact form submitted');
    });
  });
  </script>
