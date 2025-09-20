---
layout: default
title: "Finance Blog | Tips & News | The Loan Phone"
meta_description: "Stay informed with the latest finance news, tips for managing your loans, and insights into the Australian lending market from The Loan Phone blog."
meta_keywords: "finance blog, loan tips, saving money, credit score tips, australian finance news"
permalink: /blog/
---

<!-- Blog Index Content -->
<div class="bg-[#fce8e8] transition-colors duration-300">
    <div class="container mx-auto px-6 py-20 text-center">
        <div class="animate-on-scroll">
            <h1 class="text-5xl font-extrabold text-gray-800 mb-4">The Loan Phone <span style="color: #DC2626;">Blog</span></h1>
            <p class="text-xl text-gray-600 max-w-3xl mx-auto">Your source for finance tips, industry news, and guides to help you make smarter financial decisions.</p>
        </div>
    </div>
</div>

<!-- Blog Posts Section -->
<section class="py-20 bg-white transition-colors duration-300">
    <div class="container mx-auto px-6">
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            {% for post in site.posts limit: 12 %}
            <div class="bg-gray-50 rounded-lg shadow-md overflow-hidden animate-on-scroll{% cycle ' delay-1', ' delay-2', '' %}">
                {% if post.featured_image %}
                <img src="{{ site.baseurl }}/assets/images/blog/{{ post.featured_image }}" alt="{{ post.title }}" class="w-full h-48 object-cover">
                {% else %}
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-{{ post.icon | default: 'newspaper' }} text-4xl text-gray-400"></i>
                </div>
                {% endif %}
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-gray-800">{{ post.title }}</h3>
                    {% if post.excerpt %}
                    <p class="text-gray-600 mb-4">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
                    {% else %}
                    <p class="text-gray-600 mb-4">{{ post.content | strip_html | truncatewords: 25 }}</p>
                    {% endif %}
                    <div class="flex justify-between items-center">
                        <a href="{{ site.baseurl }}{{ post.url }}" class="font-semibold hover:underline" style="color: #DC2626;">Read More &rarr;</a>
                        <span class="text-sm text-gray-500">{{ post.date | date: "%B %d, %Y" }}</span>
                    </div>
                </div>
            </div>
            {% endfor %}
            
            {% if site.posts.size == 0 %}
            <!-- Placeholder blog posts if no posts exist yet -->
            <div class="bg-gray-50 rounded-lg shadow-md overflow-hidden animate-on-scroll">
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-chart-line text-4xl text-gray-400"></i>
                </div>
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-gray-800">5 Tips to Improve Your Credit Score</h3>
                    <p class="text-gray-600 mb-4">A healthy credit score is key to unlocking better loan rates. Here are five simple steps you can take today...</p>
                    <div class="flex justify-between items-center">
                        <span class="font-semibold" style="color: #DC2626;">Coming Soon</span>
                        <span class="text-sm text-gray-500">January 2025</span>
                    </div>
                </div>
            </div>
            
            <div class="bg-gray-50 rounded-lg shadow-md overflow-hidden animate-on-scroll delay-1">
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-car text-4xl text-gray-400"></i>
                </div>
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-gray-800">New vs. Used Car: Which is Cheaper to Finance?</h3>
                    <p class="text-gray-600 mb-4">The sticker price is just the beginning. We break down the true cost of financing a new versus a used vehicle...</p>
                    <div class="flex justify-between items-center">
                        <span class="font-semibold" style="color: #DC2626;">Coming Soon</span>
                        <span class="text-sm text-gray-500">January 2025</span>
                    </div>
                </div>
            </div>
            
            <div class="bg-gray-50 rounded-lg shadow-md overflow-hidden animate-on-scroll delay-2">
                <div class="w-full h-48 bg-gray-200 flex items-center justify-center">
                    <i class="fas fa-percentage text-4xl text-gray-400"></i>
                </div>
                <div class="p-6">
                    <h3 class="text-xl font-bold mb-2 text-gray-800">Understanding Fixed vs. Variable Interest Rates</h3>
                    <p class="text-gray-600 mb-4">One of the biggest decisions when getting a loan. What's the difference, and which one is right for you? Let's find out...</p>
                    <div class="flex justify-between items-center">
                        <span class="font-semibold" style="color: #DC2626;">Coming Soon</span>
                        <span class="text-sm text-gray-500">January 2025</span>
                    </div>
                </div>
            </div>
            {% endif %}
        </div>
        
        <!-- Pagination if needed -->
        {% if paginator.total_pages > 1 %}
        <div class="flex justify-center mt-12">
            <nav class="flex space-x-2">
                {% if paginator.previous_page %}
                <a href="{{ paginator.previous_page_path | prepend: site.baseurl }}" class="px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">Previous</a>
                {% endif %}
                
                {% for page in (1..paginator.total_pages) %}
                    {% if page == paginator.page %}
                    <span class="px-4 py-2 bg-red-600 text-white rounded">{{ page }}</span>
                    {% elsif page == 1 %}
                    <a href="{{ '/blog/' | prepend: site.baseurl }}" class="px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">{{ page }}</a>
                    {% else %}
                    <a href="{{ site.paginate_path | replace: ':num', page | prepend: site.baseurl }}" class="px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">{{ page }}</a>
                    {% endif %}
                {% endfor %}
                
                {% if paginator.next_page %}
                <a href="{{ paginator.next_page_path | prepend: site.baseurl }}" class="px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">Next</a>
                {% endif %}
            </nav>
        </div>
        {% endif %}
    </div>
</section>

<style>
.animate-on-scroll { 
    opacity: 0; 
    transform: translateY(20px); 
    transition: opacity 0.6s ease-out, transform 0.6s ease-out; 
}
.animate-on-scroll.is-visible { 
    opacity: 1; 
    transform: translateY(0); 
}
.delay-1 { transition-delay: 0.1s; } 
.delay-2 { transition-delay: 0.2s; }
</style>

<script>
// Animation on scroll
document.addEventListener('DOMContentLoaded', () => {
    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => { 
            if (entry.isIntersecting) { 
                entry.target.classList.add('is-visible'); 
            } 
        });
    }, { threshold: 0.1 });
    
    const elementsToAnimate = document.querySelectorAll('.animate-on-scroll');
    elementsToAnimate.forEach(el => observer.observe(el));
});
</script>
