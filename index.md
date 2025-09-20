---
layout: default
title: "Compare Loans FAST with No Impact | The Loan Phone"
meta_description: "Compare Car Loans, Personal Loans, Home Loans, Investment Loans, or Business Loans with zero impact on your credit score. Best personalised rates from 100+ lenders."
meta_keywords: "car loans, personal loans, home loans, investment loans, business loans, refinance, best loan rates"
meta_author: "The Loan Phone Team"
og_title: "Compare Loans FAST | The Loan Phone"
og_description: "Get personalised best loan rates from 100+ lenders with no credit score impact."
og_type: "website"
og_image: "/assets/images/loan-hero.jpg"
twitter_title: "Compare Loans FAST | The Loan Phone"
twitter_description: "Find the best loans personalised for you with zero impact on credit score."
twitter_image: "/assets/images/loan-twitter.jpg"
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
    <div id="loan-selector" class="bg-[var(--bg-primary)] p-4 sm:p-8 rounded-2xl shadow-2xl animate-on-scroll delay-3">
      <h3 class="text-xl font-bold text-center mb-4 text-[var(--text-primary)]">What type of loan do you need?</h3>
      <div class="grid grid-cols-2 sm:grid-cols-3 gap-4">
        {% for loan in site.data.loan-types.main_categories %}
          <a href="{{ site.baseurl }}{{ loan.url }}" class="text-center p-4 bg-[var(--bg-secondary)] rounded-lg cursor-pointer hover:shadow-md transition-shadow">
            <i class="{{ loan.icon }} text-3xl brand-red mb-2"></i>
            <p class="font-semibold text-sm text-[var(--text-secondary)]">{{ loan.name }}</p>
          </a>
        {% endfor %}
      </div>
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
    <div class="aspect-video max-w-4xl mx-auto bg-black rounded-lg shadow-2xl overflow-hidden animate-on-scroll delay-2">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/6skCwdEYgPc?si=EzTFEyOQ9SLzpVhJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen class="w-full h-full"></iframe>
    </div>
  </div>
</section>

<section id="loan-types" class="py-20 bg-[var(--bg-secondary)] transition-colors duration-300">
  <div class="container mx-auto px-6">
    <h2 class="text-3xl font-bold text-center mb-12 animate-on-scroll">Covering All Your Loan Needs</h2>
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-8 text-center text-[var(--text-secondary)] animate-on-scroll delay-1">
      {% for loan in site.data.loan-types.all_types %}
        <a href="{{ site.baseurl }}{{ loan.url }}" class="hover:brand-red font-semibold">{{ loan.name }}</a>
      {% endfor %}
    </div>
  </div>
</section>---
layout: default
title: "Compare Loans FAST with No Impact | The Loan Phone"
meta_description: "Compare Car Loans, Personal Loans, Home Loans, Investment Loans, or Business Loans with zero impact on your credit score. Best personalised rates from 100+ lenders."
meta_keywords: "car loans, personal loans, home loans, investment loans, business loans, refinance, best loan rates"
meta_author: "The Loan Phone Team"
og_title: "Compare Loans FAST | The Loan Phone"
og_description: "Get personalised best loan rates from 100+ lenders with no credit score impact."
og_type: "website"
og_image: "/assets/images/loan-hero.jpg"
twitter_title: "Compare Loans FAST | The Loan Phone"
twitter_description: "Find the best loans personalised for you with zero impact on credit score."
twitter_image: "/assets/images/loan-twitter.jpg"
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
    <div id="loan-selector" class="bg-[var(--bg-primary)] p-4 sm:p-8 rounded-2xl shadow-2xl animate-on-scroll delay-3">
      <h3 class="text-xl font-bold text-center mb-4 text-[var(--text-primary)]">What type of loan do you need?</h3>
      <div class="grid grid-cols-2 sm:grid-cols-3 gap-4">
        {% for loan in site.data.loan-types.main_categories %}
          <a href="{{ site.baseurl }}{{ loan.url }}" class="text-center p-4 bg-[var(--bg-secondary)] rounded-lg cursor-pointer hover:shadow-md transition-shadow">
            <i class="{{ loan.icon }} text-3xl brand-red mb-2"></i>
            <p class="font-semibold text-sm text-[var(--text-secondary)]">{{ loan.name }}</p>
          </a>
        {% endfor %}
      </div>
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
    <div class="aspect-video max-w-4xl mx-auto bg-black rounded-lg shadow-2xl overflow-hidden animate-on-scroll delay-2">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/6skCwdEYgPc?si=EzTFEyOQ9SLzpVhJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen class="w-full h-full"></iframe>
    </div>
  </div>
</section>

<section id="loan-types" class="py-20 bg-[var(--bg-secondary)] transition-colors duration-300">
  <div class="container mx-auto px-6">
    <h2 class="text-3xl font-bold text-center mb-12 animate-on-scroll">Covering All Your Loan Needs</h2>
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-8 text-center text-[var(--text-secondary)] animate-on-scroll delay-1">
      {% for loan in site.data.loan-types.all_types %}
        <a href="{{ site.baseurl }}{{ loan.url }}" class="hover:brand-red font-semibold">{{ loan.name }}</a>
      {% endfor %}
    </div>
  </div>
</section>
