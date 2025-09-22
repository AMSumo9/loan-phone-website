---
layout: default
title: "Thank You | The Loan Phone"
meta_description: "Thank you for your inquiry. A loan specialist will contact you shortly to discuss your loan options."
meta_keywords: "thank you, loan inquiry, contact, loan specialist"
permalink: /thank-you/
---

<!-- Thank You Hero Section -->
<section class="bg-[var(--bg-accent)] transition-colors duration-300">
    <div class="container mx-auto px-6 py-16 text-center animate-on-scroll">
        <div class="max-w-3xl mx-auto">
            <i class="fas fa-check-circle text-6xl brand-red mb-6"></i>
            <h1 class="text-5xl font-extrabold text-[var(--text-primary)] mb-4">Thank You!</h1>
            <p class="text-xl text-[var(--text-secondary)] mb-6">
                Your inquiry has been received successfully. A loan specialist will contact you shortly.
            </p>
        </div>
    </div>
</section>

<!-- Main Content -->
<section class="py-16 bg-[var(--bg-primary)] transition-colors duration-300">
    <div class="container mx-auto px-6">
        <div class="max-w-4xl mx-auto">
            
            <!-- What Happens Next -->
            <div class="bg-white rounded-lg shadow-lg p-8 mb-8">
                <h2 class="text-3xl font-bold text-[var(--text-primary)] text-center mb-8">What Happens Next?</h2>
                
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="text-center">
                        <div class="bg-red-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-phone text-2xl brand-red"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">1. We'll Call You</h3>
                        <p class="text-[var(--text-secondary)]">A qualified loan specialist will contact you within 24 hours to discuss your requirements.</p>
                    </div>
                    
                    <div class="text-center">
                        <div class="bg-red-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-search text-2xl brand-red"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">2. We Find Options</h3>
                        <p class="text-[var(--text-secondary)]">We'll search our network of lenders to find the best loan options for your situation.</p>
                    </div>
                    
                    <div class="text-center">
                        <div class="bg-red-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-handshake text-2xl brand-red"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">3. You Choose</h3>
                        <p class="text-[var(--text-secondary)]">We'll present your options and help you choose the loan that works best for you.</p>
                    </div>
                </div>
            </div>

            <!-- Quick Contact Options -->
            <div class="bg-white rounded-lg shadow-lg p-8 mb-8">
                <h2 class="text-2xl font-bold text-[var(--text-primary)] text-center mb-6">Need to Speak with Someone Right Away?</h2>
                
                <div class="grid md:grid-cols-2 gap-6">
                    <div class="text-center">
                        <a href="tel:{{ site.contact.phone }}" class="inline-block w-full px-6 py-4 rounded-lg font-semibold transition duration-300 text-gray-800" style="background-color: #fce8e8;">
                            <i class="fas fa-phone mr-2"></i>
                            Call {{ site.contact.phone_display }}
                        </a>
                        <p class="text-sm text-[var(--text-secondary)] mt-2">Speak directly with a loan specialist</p>
                    </div>
                    
                    <div class="text-center">
                        <a href="mailto:{{ site.contact.email }}" class="inline-block w-full border-2 px-6 py-4 rounded-lg font-semibold transition duration-300" style="border-color: #fce8e8; color: #374151;">
                            <i class="fas fa-envelope mr-2"></i>
                            Email Us
                        </a>
                        <p class="text-sm text-[var(--text-secondary)] mt-2">Send us a message anytime</p>
                    </div>
                </div>
            </div>

            <!-- While You Wait -->
            <div class="bg-white rounded-lg shadow-lg p-8 mb-8">
                <h2 class="text-2xl font-bold text-[var(--text-primary)] text-center mb-6">While You Wait</h2>
                
                <div class="grid md:grid-cols-2 gap-8">
                    <div>
                        <h3 class="text-lg font-bold mb-4"><i class="fas fa-book mr-2 brand-red"></i> Learn More</h3>
                        <ul class="space-y-2">
                            <li><a href="{{ site.baseurl }}/blog/" class="text-[var(--text-secondary)] hover:text-red-600">Read our latest loan tips and guides</a></li>
                            <li><a href="{{ site.baseurl }}/about/" class="text-[var(--text-secondary)] hover:text-red-600">Learn about our company and team</a></li>
                            <li><a href="{{ site.baseurl }}/services/" class="text-[var(--text-secondary)] hover:text-red-600">Browse all our loan services</a></li>
                        </ul>
                    </div>
                    
                    <div>
                        <h3 class="text-lg font-bold mb-4"><i class="fas fa-calculator mr-2 brand-red"></i> Prepare</h3>
                        <ul class="space-y-2">
                            <li class="text-[var(--text-secondary)]">Gather your financial documents</li>
                            <li class="text-[var(--text-secondary)]">Think about your loan requirements</li>
                            <li class="text-[var(--text-secondary)]">Prepare any questions you might have</li>
                        </ul>
                    </div>
                </div>
            </div>

            <!-- Navigation Options -->
            <div class="text-center">
                <h2 class="text-2xl font-bold text-[var(--text-primary)] mb-6">Continue Browsing</h2>
                <div class="flex flex-wrap justify-center gap-4">
                    <a href="{{ site.baseurl }}/" class="px-6 py-3 border-2 rounded-lg font-semibold transition duration-300 hover:bg-red-50" style="border-color: #fce8e8; color: #374151;">
                        <i class="fas fa-home mr-2"></i>
                        Home
                    </a>
                    <a href="{{ site.baseurl }}/services/" class="px-6 py-3 border-2 rounded-lg font-semibold transition duration-300 hover:bg-red-50" style="border-color: #fce8e8; color: #374151;">
                        <i class="fas fa-list mr-2"></i>
                        All Services
                    </a>
                    <a href="{{ site.baseurl }}/blog/" class="px-6 py-3 border-2 rounded-lg font-semibold transition duration-300 hover:bg-red-50" style="border-color: #fce8e8; color: #374151;">
                        <i class="fas fa-newspaper mr-2"></i>
                        Blog
                    </a>
                </div>
            </div>
        </div>
    </div>
</section>
