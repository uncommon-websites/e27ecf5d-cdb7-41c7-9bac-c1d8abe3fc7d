<script lang="ts">
  import Navbar from '$lib/components/Navbar.svelte';

  const services = [
    {
      title: "Custom AI Solutions",
      description: "Tailored AI software built specifically for your business needs"
    },
    {
      title: "Process Automation",
      description: "Streamline operations with intelligent automation systems"
    },
    {
      title: "Data Intelligence",
      description: "Transform your data into actionable business insights"
    }
  ];

  const teamMembers = [
    {
      name: "Expert AI Engineers",
      role: "Building cutting-edge solutions"
    },
    {
      name: "Business Strategists",
      role: "Understanding your needs"
    },
    {
      name: "Technical Architects",
      role: "Designing scalable systems"
    }
  ];
</script>

<style>
  .hero-gradient {
    background: linear-gradient(135deg, #2563EB 0%, #0EA5E9 50%, #06B6D4 100%);
  }
  
  .card-gradient-1 {
    background: linear-gradient(135deg, #60A5FA 0%, #0EA5E9 100%);
  }
  
  .card-gradient-2 {
    background: linear-gradient(135deg, #06B6D4 0%, #14B8A6 100%);
  }
  
  .card-gradient-3 {
    background: linear-gradient(135deg, #4F46E5 0%, #2563EB 100%);
  }

  .text-gradient {
    background: linear-gradient(135deg, #2563EB 0%, #0EA5E9 50%, #06B6D4 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .glow-blue {
    box-shadow: 0 0 60px rgba(37, 99, 235, 0.3);
  }

  .glow-cyan {
    box-shadow: 0 0 60px rgba(6, 182, 212, 0.3);
  }
</style>

<Navbar />

<div class="w-full bg-white">
  <!-- Hero Section -->
  <main class="w-full pt-32 md:pt-40 pb-20 px-4 relative overflow-hidden">
    <!-- Gradient Background Orbs -->
    <div class="absolute top-0 right-0 w-[600px] h-[600px] rounded-full hero-gradient opacity-20 blur-3xl"></div>
    <div class="absolute bottom-0 left-0 w-[500px] h-[500px] rounded-full bg-gradient-to-br from-blue-500 to-cyan-500 opacity-15 blur-3xl"></div>
    
    <div class="max-w-7xl mx-auto relative z-10">
      <div class="text-center mb-16">
        <!-- Badge -->
        <div class="inline-flex items-center gap-2 bg-blue-50 border border-blue-200 rounded-full px-4 py-2 mb-8">
          <span class="w-2 h-2 rounded-full bg-blue-500 animate-pulse"></span>
          <span class="text-sm font-semibold text-blue-700">AI product studio for small to medium businesses</span>
        </div>
        
        <h1 class="text-5xl md:text-7xl lg:text-8xl font-bold mb-8 leading-[1.1]">
          Custom AI software<br>
          <span class="text-gradient">built for your business</span>
        </h1>
        
        <p class="text-xl md:text-2xl text-gray-600 max-w-3xl mx-auto mb-12 leading-relaxed">
          We're a consultancy of three expert engineers who build tailored AI solutions that solve your unique business challenges.
        </p>
        
        <!-- CTA Buttons -->
        <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-16">
          <a href="#" class="group relative inline-flex items-center gap-2 bg-gradient-to-r from-blue-600 to-cyan-600 text-white px-8 py-4 rounded-full font-bold text-lg transition-all hover:scale-105 hover:shadow-2xl glow-blue">
            Start your project
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" class="group-hover:translate-x-1 transition-transform"><path d="m9 18 6-6-6-6"/></svg>
          </a>
          <a href="#" class="inline-flex items-center gap-2 bg-white border-2 border-gray-200 text-gray-900 px-8 py-4 rounded-full font-bold text-lg transition-all hover:border-blue-300 hover:bg-blue-50">
            View our work
          </a>
        </div>
      </div>

      <!-- Hero Cards -->
      <div class="grid md:grid-cols-3 gap-6 max-w-6xl mx-auto">
        <!-- Card 1 -->
        <div class="card-gradient-1 rounded-3xl p-8 text-white transform hover:scale-105 transition-all glow-blue">
          <div class="w-12 h-12 bg-white/20 rounded-2xl flex items-center justify-center mb-6 backdrop-blur-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="3" width="20" height="14" rx="2" ry="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg>
          </div>
          <h3 class="text-2xl font-bold mb-3">Custom built</h3>
          <p class="text-white/90 leading-relaxed">Every solution is designed specifically for your business needs</p>
        </div>

        <!-- Card 2 -->
        <div class="card-gradient-2 rounded-3xl p-8 text-white transform hover:scale-105 transition-all">
          <div class="w-12 h-12 bg-white/20 rounded-2xl flex items-center justify-center mb-6 backdrop-blur-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
          </div>
          <h3 class="text-2xl font-bold mb-3">Expert team</h3>
          <p class="text-white/90 leading-relaxed">Three dedicated engineers with deep AI expertise</p>
        </div>

        <!-- Card 3 -->
        <div class="card-gradient-3 rounded-3xl p-8 text-white transform hover:scale-105 transition-all glow-cyan">
          <div class="w-12 h-12 bg-white/20 rounded-2xl flex items-center justify-center mb-6 backdrop-blur-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
          </div>
          <h3 class="text-2xl font-bold mb-3">Scalable solutions</h3>
          <p class="text-white/90 leading-relaxed">Built to grow with your business from day one</p>
        </div>
      </div>
    </div>
  </main>

  <!-- Stats Section -->
  <section class="py-20 bg-gray-50">
    <div class="max-w-7xl mx-auto px-6">
      <p class="text-center text-sm text-gray-500 mb-12 uppercase tracking-wider font-bold">Delivering results for businesses</p>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-12 items-center justify-items-center">
        <div class="text-center">
          <div class="text-5xl font-bold text-gradient mb-3">3</div>
          <p class="text-gray-600 font-medium">Expert engineers</p>
        </div>
        <div class="text-center">
          <div class="text-5xl font-bold text-gradient mb-3">100%</div>
          <p class="text-gray-600 font-medium">Custom solutions</p>
        </div>
        <div class="text-center">
          <div class="text-5xl font-bold text-gradient mb-3">SMB</div>
          <p class="text-gray-600 font-medium">Focused expertise</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 1 -->
  <section class="py-32 px-6 bg-white">
    <div class="max-w-7xl mx-auto">
      <div class="grid md:grid-cols-2 gap-16 items-center">
        <!-- Content -->
        <div>
          <div class="inline-block bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm font-bold mb-6">
            AI consultancy
          </div>
          
          <h2 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
            We build AI solutions tailored to your business
          </h2>
          
          <p class="text-xl text-gray-600 mb-10 leading-relaxed">
            As a specialized consultancy, we understand that every business has unique challenges. Our team of three expert engineers designs and builds custom AI software that fits your specific needs.
          </p>

          <div class="space-y-6">
            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/><polyline points="3.27 6.96 12 12.01 20.73 6.96"/><line x1="12" y1="22.08" x2="12" y2="12"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Custom AI development</h3>
                <p class="text-gray-600 leading-relaxed">
                  We don't do templates or one-size-fits-all. Every solution is built from the ground up for your business.
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-cyan-500 to-teal-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"/><path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Designed for your workflow</h3>
                <p class="text-gray-600 leading-relaxed">
                  We take time to understand your processes and build software that enhances how you work.
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-indigo-500 to-blue-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Small team, big expertise</h3>
                <p class="text-gray-600 leading-relaxed">
                  Our team of three means you get direct access to senior engineers, not junior developers.
                </p>
              </div>
            </div>
          </div>
        </div>

        <!-- Visual -->
        <div class="relative">
          <div class="absolute inset-0 bg-gradient-to-br from-blue-500 to-cyan-500 rounded-3xl blur-3xl opacity-20"></div>
          <div class="relative bg-white rounded-3xl p-8 border-2 border-gray-100 shadow-2xl">
            <img src="/generated/image-a-student-in-a-modern-library-using-a-la-1769124077989-0.webp" alt="Team working on AI solutions" class="w-full h-full object-cover rounded-2xl" />
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section class="py-20 px-6 bg-gradient-to-br from-blue-50 to-cyan-50">
    <div class="max-w-7xl mx-auto">
      <div class="text-center mb-16">
        <div class="inline-block bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm font-bold mb-6">
          Our services
        </div>
        <h2 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
          Custom AI solutions for every business need
        </h2>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto leading-relaxed">
          We specialize in building AI software that's customized to solve your specific challenges, whether it's automation, data analysis, or intelligent decision-making.
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        {#each services as service}
          <div class="bg-white rounded-3xl p-8 border-2 border-blue-100 hover:border-blue-300 transition-all">
            <h3 class="text-2xl font-bold text-gray-900 mb-4">{service.title}</h3>
            <p class="text-gray-600 leading-relaxed">{service.description}</p>
          </div>
        {/each}
      </div>
    </div>
  </section>

  <!-- Team Section -->
  <section class="py-32 px-6 bg-white">
    <div class="max-w-7xl mx-auto">
      <div class="grid md:grid-cols-2 gap-16 items-center">
        <!-- Visual -->
        <div class="relative order-2 md:order-1">
          <div class="absolute inset-0 bg-gradient-to-br from-cyan-500 to-emerald-500 rounded-3xl blur-3xl opacity-20"></div>
          <div class="relative bg-white rounded-3xl p-8 border-2 border-gray-100 shadow-2xl">
            <img src="/generated/image-a-close-up-of-a-tablet-screen-showing-de-1769124080812-1.webp" alt="Our team of three engineers" class="w-full h-full object-cover rounded-2xl" />
          </div>
        </div>

        <!-- Content -->
        <div class="order-1 md:order-2">
          <div class="inline-block bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm font-bold mb-6">
            Our team
          </div>
          
          <h2 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
            A team of three, dedicated to your success
          </h2>
          
          <p class="text-xl text-gray-600 mb-10 leading-relaxed">
            We're a lean, focused team of three expert engineers. This means you work directly with senior talent who understand both AI technology and business strategy.
          </p>

          <div class="space-y-6">
            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Senior engineers only</h3>
                <p class="text-gray-600 leading-relaxed">
                  No junior developers or outsourcing. You get experienced engineers on every project.
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-cyan-500 to-teal-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Direct communication</h3>
                <p class="text-gray-600 leading-relaxed">
                  Work directly with the people building your software. No account managers or middlemen.
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-indigo-500 to-blue-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Focused on quality</h3>
                <p class="text-gray-600 leading-relaxed">
                  We take on fewer projects to ensure each one gets the attention it deserves.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Process Section -->
  <section class="py-32 px-6 bg-gray-50">
    <div class="max-w-7xl mx-auto">
      <div class="text-center mb-20">
        <div class="inline-block bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm font-bold mb-6">
          How we work
        </div>
        <h2 class="text-4xl md:text-6xl font-bold mb-6">Built around your business needs</h2>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto">Every project starts with understanding your unique challenges. We then design and build a custom AI solution that fits perfectly into your workflow.</p>
      </div>

      <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
        <!-- Step 1 -->
        <div class="bg-white rounded-3xl p-8 border-2 border-gray-200 flex flex-col">
          <div class="w-16 h-16 rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center mb-6">
            <span class="text-3xl font-bold text-white">1</span>
          </div>
          <h3 class="text-2xl font-bold text-gray-900 mb-4">Discovery</h3>
          <p class="text-gray-600 leading-relaxed">We dive deep into your business processes, challenges, and goals to understand exactly what you need.</p>
        </div>

        <!-- Step 2 -->
        <div class="bg-white rounded-3xl p-8 border-2 border-gray-200 flex flex-col">
          <div class="w-16 h-16 rounded-2xl bg-gradient-to-br from-cyan-500 to-teal-500 flex items-center justify-center mb-6">
            <span class="text-3xl font-bold text-white">2</span>
          </div>
          <h3 class="text-2xl font-bold text-gray-900 mb-4">Design</h3>
          <p class="text-gray-600 leading-relaxed">We design a custom AI solution tailored to your specific requirements and business workflow.</p>
        </div>

        <!-- Step 3 -->
        <div class="bg-white rounded-3xl p-8 border-2 border-gray-200 flex flex-col">
          <div class="w-16 h-16 rounded-2xl bg-gradient-to-br from-indigo-500 to-blue-500 flex items-center justify-center mb-6">
            <span class="text-3xl font-bold text-white">3</span>
          </div>
          <h3 class="text-2xl font-bold text-gray-900 mb-4">Build & Deploy</h3>
          <p class="text-gray-600 leading-relaxed">We build your custom software and deploy it seamlessly into your existing systems.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section class="py-32 px-6 text-center relative overflow-hidden">
    <div class="absolute inset-0 hero-gradient opacity-95"></div>
    <div class="absolute inset-0">
      <div class="absolute top-10 left-10 w-72 h-72 bg-white/10 rounded-full blur-3xl"></div>
      <div class="absolute bottom-10 right-10 w-96 h-96 bg-white/10 rounded-full blur-3xl"></div>
    </div>
    
    <div class="max-w-4xl mx-auto relative z-10">
      <h2 class="text-5xl md:text-6xl font-bold mb-8 text-white leading-tight">
        Ready to transform your<br>business with AI?
      </h2>
      <p class="text-xl md:text-2xl text-white/90 max-w-2xl mx-auto mb-12 leading-relaxed">
        Let's discuss how custom AI software can solve your unique business challenges. Our team of three is ready to build your solution.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <a href="#" class="group inline-flex items-center gap-2 bg-white text-blue-600 px-10 py-5 rounded-full font-bold text-lg transition-all hover:scale-105 shadow-2xl">
          Schedule a consultation
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" class="group-hover:translate-x-1 transition-transform"><path d="m9 18 6-6-6-6"/></svg>
        </a>
        <a href="#" class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm border-2 border-white/30 text-white px-10 py-5 rounded-full font-bold text-lg transition-all hover:bg-white/20">
          View case studies
        </a>
      </div>
      <p class="mt-8 text-white/80 text-sm">Custom solutions for small to medium businesses</p>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-900 text-white pt-20 pb-10 px-6">
    <div class="max-w-7xl mx-auto">
      <div class="grid grid-cols-2 md:grid-cols-6 gap-12 mb-16">
        <div class="col-span-2">
          <a href="/" class="flex items-center gap-2 mb-6">
            <div class="w-10 h-10 rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM12 20C7.59 20 4 16.41 4 12C4 7.59 7.59 4 12 4C16.41 4 20 7.59 20 12C20 16.41 16.41 20 12 20Z" fill="white" opacity="0.3"/>
                <path d="M12 6C8.69 6 6 8.69 6 12C6 15.31 8.69 18 12 18C15.31 18 18 15.31 18 12C18 15.31 18 12 12 6ZM12 16C9.79 16 8 14.21 8 12C8 9.79 9.79 8 12 8C14.21 8 16 9.79 16 12C16 14.21 14.21 16 12 16Z" fill="white"/>
              </svg>
            </div>
            <span class="font-bold text-xl tracking-tight">AI Studio</span>
          </a>
          <p class="text-gray-400 max-w-xs leading-relaxed">Custom AI software solutions built by a team of three expert engineers for small to medium businesses.</p>
        </div>
        
        <div>
          <h4 class="font-bold text-white mb-4">Services</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">Custom AI development</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Process automation</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Data intelligence</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Consulting</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-bold text-white mb-4">Resources</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">Case studies</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Blog</a></li>
            <li><a href="#" class="hover:text-white transition-colors">AI insights</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Support</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-bold text-white mb-4">Company</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">About us</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Our team</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Contact</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-bold text-white mb-4">Legal</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">Privacy policy</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Terms of service</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-center pt-8 border-t border-gray-800">
        <div class="text-sm text-gray-400 mb-4 md:mb-0">
          © 2025 AI Studio. All rights reserved.
        </div>

        <div class="flex items-center gap-4">
          <a href="#" class="text-gray-400 hover:text-white transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
          </a>
          <a href="#" class="text-gray-400 hover:text-white transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
          </a>
        </div>
      </div>
    </div>
  </footer>
</div>



