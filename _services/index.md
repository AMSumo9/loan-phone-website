---
layout: services
title: "Loan Services | The Loan Phone"
meta_description: "Compare car loans, home loans, personal loans, business loans and more. Find the perfect loan solution with Australia's trusted loan comparison service."
meta_keywords: "loan services, car loans, home loans, personal loans, business loans, loan comparison, australia"
permalink: /services/
---

# Our Loan Services

At The Loan Phone, we specialize in helping Australians find the perfect loan solution. Whether you're buying a car, purchasing a home, expanding your business, or need personal finance, we connect you with competitive rates from trusted lenders across Australia.

## How Our Service Works

1. **Tell Us What You Need** - Share your loan requirements with our expert team
2. **We Do the Hard Work** - We compare rates and terms from multiple lenders
3. **Get Your Best Options** - Receive tailored loan recommendations that suit your situation
4. **Make Your Choice** - Choose the loan that works best for you

---

## Featured Services

{% assign featured_services = site.services | where: "featured", true | sort: "order" %}

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 my-8">

{% if featured_services.size > 0 %}
  {% for service in featured_services limit: 6 %}
  <div class="bg-gradient-to-br from-blue-50 to-blue-100 p-6 rounded-lg shadow-lg hover:shadow-xl transition duration-300">
    <div class="flex items-center mb-4">
      {% if service.icon %}
      <i class="{{ service.icon }} text-3xl text-blue-600 mr-4"></i>
      {% endif %}
      <h3 class="text-xl font-bold text-blue-800">{{ service.title | remove: ' | The Loan Phone' }}</h3>
    </div>
    <p class="text-gray-700 mb-4">{{ service.excerpt | default: service.meta_description }}</p>
    <a href="{{ service.url }}" class="inline-flex items-center text-blue-600 font-semibold hover:text-blue-800">
      Learn More <i class="fas fa-arrow-right ml-2"></i>
    </a>
  </div>
  {% endfor %}
{% else %}
  <!-- Fallback featured services -->
  <div class="bg-blue-50 p-6 rounded-lg shadow-lg">
    <h3 class="text-xl font-bold text-blue-800 mb-3">New Car Loans</h3>
    <p class="text-gray-700 mb-4">Get competitive rates and flexible terms for your new vehicle purchase</p>
    <a href="{{ site.baseurl }}/new-car-loans/" class="text-blue-600 font-semibold hover:text-blue-800">Learn More →</a>
  </div>
  <div class="bg-green-50 p-6 rounded-lg shadow-lg">
    <h3 class="text-xl font-bold text-green-800 mb-3">Home Loans</h3>
    <p class="text-gray-700 mb-4">Find competitive mortgage rates for your home purchase or refinance</p>
    <a href="{{ site.baseurl }}/home-loans/" class="text-green-600 font-semibold hover:text-green-800">Learn More →</a>
  </div>
  <div class="bg-purple-50 p-6 rounded-lg shadow-lg">
    <h3 class="text-xl font-bold text-purple-800 mb-3">Business Loans</h3>
    <p class="text-gray-700 mb-4">Grow your business with tailored finance solutions</p>
    <a href="{{ site.baseurl }}/business-loans/" class="text-purple-600 font-semibold hover:text-purple-800">Learn More →</a>
  </div>
{% endif %}

</div>

---

## All Services by Category

{% assign home_services = site.services | where: "category", "home" | sort: "order" %}
{% assign vehicle_services = site.services | where: "category", "vehicle" | sort: "order" %}
{% assign business_services = site.services | where: "category", "business" | sort: "order" %}
{% assign personal_services = site.services | where: "category", "personal" | sort: "order" %}
{% assign specialty_services = site.services | where: "category", "specialty" | sort: "order" %}

<div class="grid grid-cols-1 lg:grid-cols-2 gap-8 my-12">

{% if home_services.size > 0 %}
<div class="bg-gradient-to-br from-blue-50 to-blue-100 p-8 rounded-lg shadow-lg">
  <div class="flex items-center mb-6">
    <i class="fas fa-home text-3xl text-blue-600 mr-4"></i>
    <h3 class="text-2xl font-bold text-blue-800">Home & Property</h3>
  </div>
  <p class="text-gray-700 mb-6">Perfect for first-time buyers, upgraders, investors, or home improvers.</p>
  <ul class="space-y-3">
    {% for service in home_services %}
    <li>
      <a href="{{ service.url }}" class="flex items-center text-blue-700 hover:text-blue-900 font-medium group">
        <i class="fas fa-chevron-right mr-2 group-hover:transform group-hover:translate-x-1 transition duration-200"></i>
        {{ service.title | remove: ' | The Loan Phone' }}
      </a>
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if vehicle_services.size > 0 %}
<div class="bg-gradient-to-br from-green-50 to-green-100 p-8 rounded-lg shadow-lg">
  <div class="flex items-center mb-6">
    <i class="fas fa-car text-3xl text-green-600 mr-4"></i>
    <h3 class="text-2xl font-bold text-green-800">Vehicle Finance</h3>
  </div>
  <p class="text-gray-700 mb-6">Get behind the wheel with competitive car and truck finance options.</p>
  <ul class="space-y-3">
    {% for service in vehicle_services %}
    <li>
      <a href="{{ service.url }}" class="flex items-center text-green-700 hover:text-green-900 font-medium group">
        <i class="fas fa-chevron-right mr-2 group-hover:transform group-hover:translate-x-1 transition duration-200"></i>
        {{ service.title | remove: ' | The Loan Phone' }}
      </a>
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if business_services.size > 0 %}
<div class="bg-gradient-to-br from-purple-50 to-purple-100 p-8 rounded-lg shadow-lg">
  <div class="flex items-center mb-6">
    <i class="fas fa-briefcase text-3xl text-purple-600 mr-4"></i>
    <h3 class="text-2xl font-bold text-purple-800">Business Finance</h3>
  </div>
  <p class="text-gray-700 mb-6">Grow your business with tailored finance solutions.</p>
  <ul class="space-y-3">
    {% for service in business_services %}
    <li>
      <a href="{{ service.url }}" class="flex items-center text-purple-700 hover:text-purple-900 font-medium group">
        <i class="fas fa-chevron-right mr-2 group-hover:transform group-hover:translate-x-1 transition duration-200"></i>
        {{ service.title | remove: ' | The Loan Phone' }}
      </a>
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if personal_services.size > 0 %}
<div class="bg-gradient-to-br from-orange-50 to-orange-100 p-8 rounded-lg shadow-lg">
  <div class="flex items-center mb-6">
    <i class="fas fa-user text-3xl text-orange-600 mr-4"></i>
    <h3 class="text-2xl font-bold text-orange-800">Personal Finance</h3>
  </div>
  <p class="text-gray-700 mb-6">Life happens - we're here to help with personal loan solutions.</p>
  <ul class="space-y-3">
    {% for service in personal_services %}
    <li>
      <a href="{{ service.url }}" class="flex items-center text-orange-700 hover:text-orange-900 font-medium group">
        <i class="fas fa-chevron-right mr-2 group-hover:transform group-hover:translate-x-1 transition duration-200"></i>
        {{ service.title | remove: ' | The Loan Phone' }}
      </a>
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

</div>

{% if specialty_services.size > 0 %}
<div class="bg-gradient-to-br from-teal-50 to-teal-100 p-8 rounded-lg shadow-lg my-8">
  <div class="flex items-center mb-6">
    <i class="fas fa-leaf text-3xl text-teal-600 mr-4"></i>
    <h3 class="text-2xl font-bold text-teal-800">Specialty Finance</h3>
  </div>
  <p class="text-gray-700 mb-6">Unique loan solutions for modern Australians and specific needs.</p>
  <ul class="space-y-3">
    {% for service in specialty_services %}
    <li>
      <a href="{{ service.url }}" class="flex items-center text-teal-700 hover:text-teal-900 font-medium group">
        <i class="fas fa-chevron-right mr-2 group-hover:transform group-hover:translate-x-1 transition duration-200"></i>
        {{ service.title | remove: ' | The Loan Phone' }}
      </a>
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

---

## Complete Service Directory

{% assign all_services = site.services | sort: "title" %}

<div class="bg-gray-50 p-8 rounded-lg shadow-lg my-8">
  <h3 class="text-2xl font-bold text-gray-800 mb-6 text-center">All Available Services</h3>
  {% if all_services.size > 0 %}
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
    {% for service in all_services %}
    <a href="{{ service.url }}" class="flex items-center p-4 bg-white rounded-lg hover:bg-blue-50 hover:text-blue-700 transition duration-200 shadow-sm hover:shadow-md group">
      {% if service.icon %}
      <i class="{{ service.icon }} text-blue-500 mr-3"></i>
      {% else %}
      <i class="fas fa-arrow-right text-blue-500 mr-3"></i>
      {% endif %}
      <span class="font-medium">{{ service.title | remove: ' | The Loan Phone' }}</span>
      <i class="fas fa-external-link-alt ml-auto text-gray-400 group-hover:text-blue-500 text-sm"></i>
    </a>
    {% endfor %}
  </div>
  {% else %}
  <!-- Fallback to data file -->
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
    {% for loan_type in site.data.loan_types.all_types %}
    <a href="{{ site.baseurl }}{{ loan_type.url }}" class="flex items-center p-4 bg-white rounded-lg hover:bg-blue-50 hover:text-blue-700 transition duration-200 shadow-sm hover:shadow-md">
      <i class="fas fa-arrow-right text-blue-500 mr-3"></i>
      <span class="font-medium">{{ loan_type.name }}</span>
    </a>
    {% endfor %}
  </div>
  {% endif %}
</div>

---

## Ready to Get Started?

<div class="bg-gradient-to-r from-blue-600 to-purple-600 text-white p-8 rounded-lg text-center my-8">
  <h3 class="text-2xl font-bold mb-4">Ready to Compare Loans?</h3>
  <p class="text-lg mb-6">Get personalized loan options in minutes</p>
  <div class="space-y-4 md:space-y-0 md:space-x-4 md:flex md:justify-center">
    <a href="tel:{{ site.contact.phone }}" class="inline-block bg-white text-blue-600 px-6 py-3 rounded-lg font-semibold hover:bg-gray-100 transition duration-300">
      Call {{ site.contact.phone_display }}
    </a>
    <button onclick="openSupportModal()" class="inline-block bg-transparent border-2 border-white text-white px-6 py-3 rounded-lg font-semibold hover:bg-white hover:text-blue-600 transition duration-300">
      Get Free Quote
    </button>
  </div>
</div>
