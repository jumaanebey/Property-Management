  ---
  layout: page
  title: "Thank You!"
  subtitle: "We've received your message"
  description: "Thank you for contacting My Property Management. We'll get
   back to you soon with a response to your inquiry."
  ---

  <div class="max-w-3xl mx-auto text-center">

  <div class="w-24 h-24 bg-green-500 rounded-full flex items-center 
  justify-center mx-auto mb-8">
    <i class="fas fa-check text-white text-3xl"></i>
  </div>

  ## Message Sent Successfully!

  Thank you for contacting **My Property Management**. We've received your
   message and will get back to you within 2-4 hours during business days.

  ### What happens next?

  1. **Quick Response**: One of our team members will review your inquiry
  and respond promptly
  2. **Personal Consultation**: For property management inquiries, we'll
  schedule a free consultation
  3. **Follow-up**: We'll provide detailed information tailored to your
  specific needs

  ---

  ### In the meantime, you might find these helpful:

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6 my-8">

  <div class="bg-white p-6 rounded-lg shadow-md text-center">
    <i class="fas fa-home text-primary text-3xl mb-4"></i>
    <h4 class="font-bold text-gray-900 mb-2">Browse Properties</h4>
    <p class="text-gray-600 text-sm mb-4">Check out our available rental
  properties</p>
    <a href="{{ '/properties/' | relative_url }}" class="text-primary 
  hover:text-blue-700 font-medium">View Properties →</a>
  </div>

  <div class="bg-white p-6 rounded-lg shadow-md text-center">
    <i class="fas fa-cogs text-primary text-3xl mb-4"></i>
    <h4 class="font-bold text-gray-900 mb-2">Our Services</h4>
    <p class="text-gray-600 text-sm mb-4">Learn about our property
  management solutions</p>
    <a href="{{ '/services/' | relative_url }}" class="text-primary 
  hover:text-blue-700 font-medium">View Services →</a>
  </div>

  <div class="bg-white p-6 rounded-lg shadow-md text-center">
    <i class="fas fa-users text-primary text-3xl mb-4"></i>
    <h4 class="font-bold text-gray-900 mb-2">About Us</h4>
    <p class="text-gray-600 text-sm mb-4">Meet our experienced property
  management team</p>
    <a href="{{ '/about/' | relative_url }}" class="text-primary 
  hover:text-blue-700 font-medium">Learn More →</a>
  </div>

  </div>

  ---

  ### Need immediate assistance?

  <div class="bg-red-50 border border-red-200 rounded-lg p-6 my-8">
    <h4 class="text-lg font-bold text-red-800 mb-2">
      <i class="fas fa-exclamation-triangle mr-2"></i>
      Emergency Maintenance
    </h4>
    <p class="text-red-700 text-sm mb-3">
      For urgent maintenance issues, don't wait for our response. Call our
   24/7 emergency line immediately:
    </p>
    <a
      href="tel:+1-555-363-7436"
      class="text-lg font-bold text-red-800 hover:text-red-900"
    >
      (555) 363-7436
    </a>
  </div>

  <div class="bg-primary text-white rounded-lg p-6">
    <h4 class="text-lg font-bold mb-2">
      <i class="fas fa-phone mr-2"></i>
      General Questions?
    </h4>
    <p class="text-blue-100 text-sm mb-3">
      You can also reach us directly during business hours:
    </p>
    <a
      href="tel:{{ site.contact.phone }}"
      class="text-lg font-bold text-white hover:text-blue-200"
    >
      {{ site.contact.phone }}
    </a>
  </div>

  </div>
