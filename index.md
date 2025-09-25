---
layout: default
title: "Compare Loans FAST with No Impact | The Loan Phone"
meta_description: "Compare Car Loans, Personal Loans, Home Loans, Investment Loans, or Business Loans with zero impact on your credit score. Best personalised rates from 100+ lenders."
meta_keywords: "car loans, personal loans, home loans, investment loans, business loans, refinance, best loan rates"
---

<section class="bg-[var(--bg-accent)] py-20 md:py-32 transition-colors duration-300">
  <div class="container mx-auto px-6 grid md:grid-cols-2 gap-12 items-center">
    <div class="text-center md:text-left">
      <h1 class="text-4xl md:text-6xl font-extrabold text-[var(--text-primary)] leading-tight mb-4 animate-on-scroll">
        Compare Loans <span class="brand-red">FAST</span> with NO IMPACT to Credit Score.
      </h1>
      <p class="text-lg text-[var(--text-secondary)] mb-8 max-w-xl mx-auto md:mx-0 animate-on-scroll delay-1">
        Compare Car Loans, Personal Loans, Home Loans, Investment Loans or Business Loans - Best Rates Personalised FOR YOU from 100+ Lenders.
      </p>
      <a href="#loan-selector" class="inline-block bg-brand-red text-white font-bold text-lg px-8 py-4 rounded-lg shadow-xl hover:bg-brand-red-dark transition-transform duration-300 transform hover:scale-105 animate-on-scroll delay-2">
        Select a Loan to Start
      </a>
    </div>
    <div id="loan-selector">
      {% if site.features.loan_widget_live %}
        <!-- Live Widget -->
        <div id="repaymentWidget"></div>
        <script>
        (function () {
          const params = new Proxy(new URLSearchParams(window.location.search), {
            get: (searchParams, prop) => searchParams.get(prop),
          });
          if (params.partnerId) {
            localStorage.setItem("externalPartnerId", params.partnerId);
          } else {
            localStorage.setItem("externalPartnerId", "{{ site.features.partner_id }}");
          }
          localStorage.setItem("sourceUrl", "{{ site.features.source_url }}");
          localStorage.setItem("source", "{{ site.company.name }}");
          localStorage.setItem("targetSystem", "SKYNET");
          localStorage.setItem("countryCode", "AU");
        })();
        </script>
        <script src="{{ site.features.widget_js }}"></script>
        <link href="{{ site.features.widget_css }}" rel="stylesheet" />
      {% else %}
        <!-- Visual Placeholder -->
        <div class="bg-[var(--bg-primary)] p-4 sm:p-8 rounded-2xl shadow-2xl animate-on-scroll delay-3">
          <h3 class="text-xl font-bold text-center mb-4 text-[var(--text-primary)]">What type of loan do you need?</h3>
          <div class="grid grid-cols-2 sm:grid-cols-3 gap-4">
            {% for loan in site.data.loan_types.main_categories %}
              <div class="text-center p-4 bg-[var(--bg-secondary)] rounded-lg hover:shadow-md transition-shadow cursor-default">
                <i class="{{ loan.icon }} text-3xl brand-red mb-2"></i>
                <p class="font-semibold text-sm text-[var(--text-secondary)]">{{ loan.name }}</p>
              </div>
            {% endfor %}
          </div>
          <div class="mt-4 text-center">
            <p class="text-xs text-[var(--text-secondary)] opacity-75">
              <i class="fas fa-eye"></i> Preview Mode - Interactive widget will replace this when live
            </p>
          </div>
        </div>
      {% endif %}
    </div>
  </div>
</section>

<section id="how-it-works" class="py-20 bg-[var(--bg-secondary)] transition-colors duration-300">
  <div class="container mx-auto px-6 text-center">
    <h2 class="text-3xl font-bold mb-4 animate-on-scroll">Only 3 Quick & Easy Steps</h2>
    <div class="grid md:grid-cols-3 gap-10 mt-12">
      <div class="flex flex-col items-center animate-on-scroll delay-1">
        <div class="bg-red-100 p-6 rounded-full mb-4">
          <i class="fa-solid fa-hand-pointer text-4xl brand-red"></i>
        </div>
        <h3 class="text-xl font-bold mb-2">1. Click & Share</h3>
        <p class="text-[var(--text-secondary)]">Click to Pick a Loan Type - Share some info about You.</p>
      </div>
      <div class="flex flex-col items-center animate-on-scroll delay-2">
        <div class="bg-red-100 p-6 rounded-full mb-4">
          <i class="fa-solid fa-right-left text-4xl brand-red"></i>
        </div>
        <h3 class="text-xl font-bold mb-2">2. Compare</h3>
        <p class="text-[var(--text-secondary)]">We provide personalised options based on real data matching.</p>
      </div>
      <div class="flex flex-col items-center animate-on-scroll delay-3">
        <div class="bg-red-100 p-6 rounded-full mb-4">
          <i class="fa-solid fa-trophy text-4xl brand-red"></i>
        </div>
        <h3 class="text-xl font-bold mb-2">3. Pick Your Winner</h3>
        <p class="text-[var(--text-secondary)]">Choose the option that works best for you. Zero pressure.</p>
      </div>
    </div>
  </div>
</section>

<section class="py-20 bg-gray-900 text-white">
  <div class="container mx-auto px-6 text-center">
    <h2 class="text-3xl font-bold mb-4 animate-on-scroll">See How we Compare Loans <span class="brand-red">FAST</span></h2>
    <p class="text-gray-300 max-w-3xl mx-auto mb-8 animate-on-scroll delay-1">Whatever Loan You need, talk to Loan Phone</p>
    
    <!-- OPTIMIZED: YouTube Click-to-Play with compressed thumbnail (saves 89.2 KiB) -->
    <div class="aspect-video max-w-4xl mx-auto bg-black rounded-lg shadow-2xl overflow-hidden animate-on-scroll delay-2">
      <div 
        class="youtube-placeholder w-full h-full" 
        onclick="loadYouTubeVideo(this)" 
        data-video-id="6skCwdEYgPc"
        style="
          position: relative;
          cursor: pointer;
          background: #000;
          display: flex;
          align-items: center;
          justify-content: center;
          width: 100%;
          height: 100%;
        "
      >
        <!-- OPTIMIZED: Use smaller, more optimized YouTube thumbnail -->
        <picture>
          <!-- WebP format for modern browsers (smaller file size) -->
          <source 
            srcset="https://i.ytimg.com/vi_webp/6skCwdEYgPc/hqdefault.webp" 
            type="image/webp"
            width="480"
            height="360"
          >
          <!-- Fallback JPEG (smaller than maxresdefault) -->
          <img 
            src="https://i.ytimg.com/vi/6skCwdEYgPc/hqdefault.jpg" 
            alt="How The Loan Phone compares loans fast - Video demonstration"
            style="
              width: 100%;
              height: 100%;
              object-fit: cover;
              position: absolute;
              top: 0;
              left: 0;
            "
            loading="lazy"
            width="480"
            height="360"
            decoding="async"
          >
        </picture>
        
        <!-- OPTIMIZED: Lightweight play button with brand colors -->
        <div style="
          position: relative;
          z-index: 2;
          background: rgba(220, 38, 38, 0.9);
          border-radius: 50%;
          width: 80px;
          height: 80px;
          display: flex;
          align-items: center;
          justify-content: center;
          transition: all 0.3s ease;
          box-shadow: 0 4px 20px rgba(0,0,0,0.3);
          cursor: pointer;
        " 
        onmouseover="this.style.transform='scale(1.1)'; this.style.background='rgba(220, 38, 38, 1)'"
        onmouseout="this.style.transform='scale(1)'; this.style.background='rgba(220, 38, 38, 0.9)'"
        aria-label="Play video: How The Loan Phone compares loans fast"
        role="button"
        tabindex="0"
        onkeydown="if(event.key==='Enter'||event.key===' ') loadYouTubeVideo(this.parentElement)"
        >
          <!-- Inline SVG instead of external icon (better performance) -->
          <svg width="32" height="32" viewBox="0 0 24 24" fill="white" style="margin-left: 3px;" aria-hidden="true">
            <path d="M8 5v14l11-7z"/>
          </svg>
        </div>

        <!-- OPTIMIZED: Simplified video title overlay -->
        <div style="
          position: absolute;
          bottom: 0;
          left: 0;
          right: 0;
          background: linear-gradient(transparent, rgba(0,0,0,0.8));
          color: white;
          padding: 30px 20px 20px;
          font-size: 18px;
          font-weight: 600;
        ">
          See How We Compare Loans FAST
        </div>
      </div>
    </div>
  </div>
</section>

<section id="loan-types" class="py-20 bg-[var(--bg-secondary)] transition-colors duration-300">
  <div class="container mx-auto px-6">
    <h2 class="text-3xl font-bold text-center mb-12 animate-on-scroll">Covering All Your Loan Needs</h2>
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-8 text-center text-[var(--text-secondary)] animate-on-scroll delay-1">
      {% for loan in site.data.loan_types.all_types %}
        <a href="{{ site.baseurl }}{{ loan.url }}" class="hover:brand-red font-semibold">{{ loan.name }}</a>
      {% endfor %}
    </div>
  </div>
</section>

<script>
// OPTIMIZED: Efficient YouTube video loader with accessibility and tracking
function loadYouTubeVideo(element) {
  const videoId = element.getAttribute('data-video-id');
  const iframe = document.createElement('iframe');
  
  iframe.src = `https://www.youtube.com/embed/${videoId}?autoplay=1&rel=0`;
  iframe.width = '480';
  iframe.height = '360';
  iframe.style.cssText = 'width:100%;height:100%;position:absolute;top:0;left:0;border:none;';
  iframe.title = 'How The Loan Phone compares loans fast - Video player';
  iframe.allow = 'accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share';
  iframe.allowFullscreen = true;
  iframe.loading = 'lazy';
  
  // Replace thumbnail with iframe efficiently
  element.style.position = 'relative';
  element.innerHTML = '';
  element.appendChild(iframe);
  
  // Track video play event (only if Facebook Pixel is loaded)
  if (typeof fbq !== 'undefined') {
    fbq('track', 'ViewContent', {
      content_name: 'Loan Comparison Video',
      content_category: 'Video Engagement',
      content_type: 'video'
    });
  }
  
  // Track with Google Analytics if available
  if (typeof gtag !== 'undefined') {
    gtag('event', 'play', {
      event_category: 'Video',
      event_label: 'Loan Comparison Demo',
      value: 1
    });
  }
}

// OPTIMIZED: Enhanced widget tracking for better conversion measurement
document.addEventListener('DOMContentLoaded', function() {
  // Widget interaction tracking variables
  let widgetViewed = false;
  let widgetInteracted = false;

  // Track widget view when it comes into viewport
  const widgetObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting && entry.intersectionRatio > 0.5 && !widgetViewed) {
        widgetViewed = true;
        if (typeof fbq !== 'undefined') {
          fbq('track', 'ViewContent', {
            content_name: 'loan_comparison_widget',
            content_category: 'widget_interaction',
            content_type: 'loan_tool'
          });
        }
      }
    });
  }, { threshold: 0.5 });

  // Track widget container
  const widgetContainer = document.querySelector('#loan-selector');
  if (widgetContainer) {
    widgetObserver.observe(widgetContainer);
    
    // Track clicks on widget container
    widgetContainer.addEventListener('click', function() {
      if (!widgetInteracted && typeof fbq !== 'undefined') {
        widgetInteracted = true;
        fbq('track', 'Search', {
          search_string: 'loan_comparison',
          content_category: 'widget_start',
          content_type: 'loan_comparison'
        });
      }
    });
  }

  // Track "Select a Loan to Start" button clicks
  const startButton = document.querySelector('a[href="#loan-selector"]');
  if (startButton) {
    startButton.addEventListener('click', function() {
      if (typeof fbq !== 'undefined') {
        fbq('track', 'InitiateCheckout', {
          content_name: 'start_loan_comparison',
          content_category: 'widget_start'
        });
      }
    });
  }

  // Enhanced phone click tracking
  const phoneLinks = document.querySelectorAll('a[href^="tel:"]');
  phoneLinks.forEach(link => {
    link.addEventListener('click', function() {
      if (typeof fbq !== 'undefined') {
        fbq('track', 'Contact', {
          content_name: 'Phone Click',
          content_category: 'Contact',
          content_type: 'phone_call'
        });
      }
    });
  });
});
</script>
