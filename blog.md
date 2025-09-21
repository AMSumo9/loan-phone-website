---
layout: default
title: "Finance Blog | Tips & News | The Loan Phone"
meta_description: "Stay informed with the latest finance news, tips for managing your loans, and insights into the Australian lending market from The Loan Phone blog."
meta_keywords: "finance blog, loan tips, saving money, credit score tips, australian finance news"
permalink: /blog/
---

<!-- Blog Index Content - FIXED: Dark Mode Support -->
<div class="bg-[var(--bg-accent)] transition-colors duration-300">
    <div class="container mx-auto px-6 py-20 text-center">
        <div class="animate-on-scroll">
            <h1 class="text-5xl font-extrabold text-[var(--text-primary)] mb-4">The Loan Phone <span class="brand-red">Blog</span></h1>
            <p class="text-xl text-[var(--text-secondary)] max-w-3xl mx-auto">Your source for finance tips, industry news, and guides to help you make smarter financial decisions.</p>
        </div>
    </div>
</div>

<!-- Blog Posts Section - FIXED: Dark Mode Variables -->
<section class="py-20 bg-[var(--bg-primary)] transition-colors duration-300">
    <div class="container mx-auto px-6">
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            {% for post in site.posts limit: 12 %}
            <div class="bg-[var(--bg-secondary)] rounded-lg shadow-md overflow-hidden animate-on-scroll{% cycle ' delay-1', ' delay-2', '' %} transition-colors duration-300">
                {% if post.featured_image %}
                <img src="{{ site.baseurl }}/assets/images/blog/{{ post.featured_image }}" alt="{{ post.title }}" class="w-full h-48 object-cover">
                {% else %}
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-{{ post.icon | default: 'newspaper' }} text-4xl text-gray-400"></i>
                </div>
                {% endif %}
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-[var(--text-primary)]">{{ post.title }}</h3>
                    {% if post.excerpt %}
                    <p class="text-[var(--text-secondary)] mb-4">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
                    {% else %}
                    <p class="text-[var(--text-secondary)] mb-4">{{ post.content | strip_html | truncatewords: 25 }}</p>
                    {% endif %}
                    <div class="flex justify-between items-center">
                        <a href="{{ site.baseurl }}{{ post.url }}" class="font-semibold hover:underline brand-red">Read More &rarr;</a>
                        <span class="text-sm text-gray-500">{{ post.date | date: "%B %d, %Y" }}</span>
                    </div>
                </div>
            </div>
            {% endfor %}
            
            {% if site.posts.size == 0 %}
            <!-- Placeholder blog posts if no posts exist yet - FIXED: Dark Mode -->
            <div class="bg-[var(--bg-secondary)] rounded-lg shadow-md overflow-hidden animate-on-scroll transition-colors duration-300">
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-chart-line text-4xl text-gray-400"></i>
                </div>
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-[var(--text-primary)]">5 Tips to Improve Your Credit Score</h3>
                    <p class="text-[var(--text-secondary)] mb-4">A healthy credit score is key to unlocking better loan rates. Here are five simple steps you can take today...</p>
                    <div class="flex justify-between items-center">
                        <span class="font-semibold brand-red">Coming Soon</span>
                        <span class="text-sm text-gray-500">January 2025</span>
                    </div>
                </div>
            </div>
            
            <div class="bg-[var(--bg-secondary)] rounded-lg shadow-md overflow-hidden animate-on-scroll delay-1 transition-colors duration-300">
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-car text-4xl text-gray-400"></i>
                </div>
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-[var(--text-primary)]">New vs. Used Car: Which is Cheaper to Finance?</h3>
                    <p class="text-[var(--text-secondary)] mb-4">The sticker price is just the beginning. We break down the true cost of financing a new versus a used vehicle...</p>
                    <div class="flex justify-between items-center">
                        <span class="font-semibold brand-red">Coming Soon</span>
                        <span class="text-sm text-gray-500">January 2025</span>
                    </div>
                </div>
            </div>
            
            <div class="bg-[var(--bg-secondary)] rounded-lg shadow-md overflow-hidden animate-on-scroll delay-2 transition-colors duration-300">
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-percentage text-4xl text-gray-400"></i>
                </div>
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-[var(--text-primary)]">Understanding Fixed vs. Variable Interest Rates</h3>
                    <p class="text-[var(--text-secondary)] mb-4">One of the biggest decisions when getting a loan. What's the difference, and which one is right for you? Let's find out...</p>
                    <div class="flex justify-between items-center">
                        <span class="font-semibold brand-red">Coming Soon</span>
                        <span class="text-sm text-gray-500">January 2025</span>
                    </div>
                </div>
            </div>
            {% endif %}
        </div>
        
        <!-- Pagination if needed - FIXED: Dark Mode -->
        {% if paginator.total_pages > 1 %}
        <div class="flex justify-center mt-12">
            <nav class="flex space-x-2">
                {% if paginator.previous_page %}
                <a href="{{ paginator.previous_page_path | prepend: site.baseurl }}" class="px-4 py-2 bg-[var(--bg-secondary)] rounded hover:bg-gray-300 text-[var(--text-primary)] transition-colors duration-300">Previous</a>
                {% endif %}
                
                {% for page in (1..paginator.total_pages) %}
                    {% if page == paginator.page %}
                    <span class="px-4 py-2 bg-red-600 text-white rounded">{{ page }}</span>
                    {% elsif page == 1 %}
                    <a href="{{ '/blog/' | prepend: site.baseurl }}" class="px-4 py-2 bg-[var(--bg-secondary)] rounded hover:bg-gray-300 text-[var(--text-primary)] transition-colors duration-300">{{ page }}</a>
                    {% else %}
                    <a href="{{ site.paginate_path | replace: ':num', page | prepend: site.baseurl }}" class="px-4 py-2 bg-[var(--bg-secondary)] rounded hover:bg-gray-300 text-[var(--text-primary)] transition-colors duration-300">{{ page }}</a>
                    {% endif %}
                {% endfor %}
                
                {% if paginator.next_page %}
                <a href="{{ paginator.next_page_path | prepend: site.baseurl }}" class="px-4 py-2 bg-[var(--bg-secondary)] rounded hover:bg-gray-300 text-[var(--text-primary)] transition-colors duration-300">Next</a>
                {% endif %}
            </nav>
        </div>
        {% endif %}
    </div>
</section>
