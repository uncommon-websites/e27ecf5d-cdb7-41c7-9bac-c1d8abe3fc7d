<script>
  import { onMount } from 'svelte';
  import Navbar from '$lib/components/Navbar.svelte';

  // SVGs
  const sparkleIcon = `<svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-gray-800"><path d="M12 2L14.4 9.6L22 12L14.4 14.4L12 22L9.6 14.4L2 12L9.6 9.6L12 2Z" fill="#333"/><path d="M19 17L20 20L23 21L20 22L19 25L18 22L15 21L18 20L19 17Z" fill="#333"/><path d="M5 5L6 8L9 9L6 10L5 13L4 10L1 9L4 8L5 5Z" fill="#333"/></svg>`;

  const universityLogos = [
    "Harvard", "Stanford", "Wharton", "Oxford", "Penn", "IE", "Bocconi", "Dartmouth"
  ];
</script>

<style>
  .custom-gradient-bg {
    background: linear-gradient(to bottom, #abcfe9 0%, #eef6fb 50%, #f5f7f9 100%);
  }
</style>

<Navbar />

<div class="w-full bg-white pt-10">
  <!-- Hero Section -->
  <main class="w-full pt-16 md:pt-24 pb-12">
    <div class="max-w-4xl mx-auto px-4 text-center mb-16">
        <h1 class="text-[42px] md:text-[64px] leading-[1.1] font-normal text-[#1a1a1a] tracking-tight mb-6">
            Ace your consulting<br>
            interviews with AI.
        </h1>
        <p class="text-[19px] md:text-[21px] text-[#334155] leading-relaxed max-w-2xl mx-auto font-light">
            CasePrepared delivers realistic voice AI simulations and<br class="hidden md:block">
            detailed analytics to help you land your dream offer.
        </p>
    </div>

    <!-- Hero Visual / Gradient Area -->
    <div class="mx-4 md:mx-6 lg:mx-8 rounded-t-[40px] md:rounded-t-[60px] custom-gradient-bg h-[600px] md:h-[700px] relative overflow-hidden pt-20">
        
        <!-- Cards Container -->
        <div class="flex flex-col items-center gap-5 px-4">
            
            <!-- Card 1: AI Agent Chat -->
            <div class="bg-white rounded-[32px] p-8 md:p-10 shadow-[0_4px_20px_rgba(0,0,0,0.03)] w-full max-w-[580px] relative z-20">
                <div class="flex items-center gap-2 mb-4">
                    {@html sparkleIcon}
                    <span class="text-gray-500 text-lg font-normal">AI Agent</span>
                </div>
                <div class="text-[28px] md:text-[32px] leading-tight text-[#1a1a1a] font-normal">
                    Let's start the case. How would you approach this market entry for a luxury car brand? <span class="inline-block align-bottom">📊</span>
                </div>
            </div>

            <!-- Card 2: Room Preview -->
            <div class="bg-white rounded-[32px] p-3 pr-8 shadow-[0_4px_20px_rgba(0,0,0,0.03)] w-full max-w-[580px] flex items-center gap-6 relative z-10">
                <!-- Image Placeholder -->
                <div class="w-[140px] h-[160px] shrink-0 rounded-[24px] overflow-hidden relative bg-gray-200">
                    <img src="https://placehold.co/280x320/1e40af/ffffff?text=Case+Study" alt="Consulting Case" class="w-full h-full object-cover opacity-80 mix-blend-multiply">
                    <div class="absolute inset-0 bg-gradient-to-r from-gray-300/50 to-transparent"></div>
                </div>
                
                <!-- Content -->
                <div class="flex flex-col justify-center h-full py-2">
                    <div class="text-[28px] text-[#1a1a1a] font-normal mb-1">
                        Market <span class="text-gray-400">Entry</span>
                    </div>
                    <div class="w-1.5 h-1.5 rounded-full mt-2" style="background-color: #1e40af"></div>
                </div>
            </div>
        </div>

        <div class="absolute bottom-0 left-0 w-full h-20 bg-gradient-to-t from-[#f5f7f9] to-transparent pointer-events-none"></div>
    </div>
  </main>

  <!-- Logos Section -->
  <section class="py-16 border-b border-transparent bg-[#f5f7f9]">
    <div class="max-w-[1200px] mx-auto px-6">
      <p class="text-center text-sm text-gray-500 mb-10 uppercase tracking-widest font-medium">Used by candidates at leading institutions</p>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-y-12 gap-x-8 items-center justify-items-center opacity-60 grayscale hover:grayscale-0 transition-all duration-500">
        {#each universityLogos as university}
          <div class="h-8 flex items-center"><span class="font-bold text-xl text-[#334155]">{university}</span></div>
        {/each}
      </div>
    </div>
  </section>

  <!-- Feature Section 1 -->
  <section class="py-24 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-center">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-[#f3f6f8] rounded-[32px] aspect-square relative overflow-hidden group">
          <img src="/generated/image-a-student-in-a-modern-library-using-a-la-1769124077989-0.webp" alt="Student practicing case" class="w-full h-full object-cover" />
          <div class="absolute inset-0 bg-black/5"></div>
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Realistic Voice AI Simulations
            </h2>
            <span class="bg-[#1e40af] text-white px-3 py-1.5 rounded-full text-xs font-medium uppercase tracking-wider">The Experience</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Practice with an AI that sounds, thinks, and reacts like a real interviewer. No more static text prompts—engage in dynamic, spoken case studies.
          </p>

          <div class="space-y-10">
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#1e40af]"><path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" y1="19" x2="12" y2="23"/><line x1="8" y1="23" x2="16" y2="23"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Natural Voice Interaction</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  The AI listens to your spoken responses and probes with follow-up questions, just like a McKinsey or BCG partner.
                </p>
              </div>
            </div>

            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#1e40af]"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Adaptive Difficulty</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  The simulation adapts based on your performance, pushing you harder when you're doing well and guiding you when you're stuck.
                </p>
              </div>
            </div>

            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#1e40af]"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Full Case Library</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  From M&A and Market Entry to Pricing and Growth Strategy—practice every case type you'll encounter.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial Section -->
  <section class="py-12 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="bg-[#f3f6f8] rounded-[32px] p-12 md:p-16 relative overflow-hidden">
        <div class="absolute right-0 top-0 w-1/3 h-full opacity-10 hidden lg:block">
           <img src="/generated/image-a-diverse-group-of-ambitious-business-st-1769124083087-2.webp" alt="Students" class="w-full h-full object-cover" />
        </div>
        <div class="mb-8 font-bold text-lg text-[#1e40af]">Wharton MBA Candidate</div>
        <blockquote class="text-2xl md:text-3xl font-medium leading-tight text-gray-900 mb-12 max-w-3xl relative z-10">
          "CasePrepared is a game-changer. The AI's ability to probe my logic and provide instant feedback is as close to a real human coach as it gets, but at a fraction of the cost."
        </blockquote>
        <div class="flex items-center justify-between flex-wrap gap-6 relative z-10">
          <div class="flex items-center gap-4">
            <img src="https://i.pravatar.cc/100?img=12" alt="Candidate" class="w-12 h-12 rounded-full object-cover" />
            <div>
              <div class="font-medium text-gray-900">Alex Chen</div>
              <div class="text-sm text-gray-500">Incoming Associate at MBB</div>
            </div>
          </div>
          <a href="#" class="inline-flex items-center gap-2 bg-[#1e40af] hover:opacity-90 text-white px-5 py-2.5 rounded-full text-sm font-medium transition-colors">
            Start Practicing
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 2 (Analytics) -->
  <section class="py-24 px-6 bg-[#F9F9F9]">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row-reverse gap-16 items-center">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-white rounded-[32px] aspect-square relative flex items-center justify-center p-8 shadow-sm overflow-hidden">
           <img src="/generated/image-a-close-up-of-a-tablet-screen-showing-de-1769124080812-1.webp" alt="Analytics Dashboard" class="w-full h-full object-cover" />
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Deep Post-Interview Analytics
            </h2>
            <span class="bg-[#1e40af] text-white px-3 py-1.5 rounded-full text-xs font-medium uppercase tracking-wider">The Feedback</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Don't just practice—improve. Our AI provides line-by-line analysis of your performance across four critical dimensions.
          </p>

          <div class="space-y-10">
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#1e40af]"><path d="M21.21 15.89A10 10 0 1 1 8 2.83"/><path d="M22 12A10 10 0 0 0 12 2v10z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Quantitative & Logic Scoring</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Detailed breakdown of your math accuracy, structuring logic, and insight generation capabilities.
                </p>
              </div>
            </div>

            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#1e40af]"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Communication Analysis</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Filler word detection, thinking-time analysis, and tone assessment to ensure you sound professional and confident.
                </p>
              </div>
            </div>

            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#1e40af]"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Line-by-Line Transcript</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Review exactly what you said and how the AI responded, with specific suggestions for better phrasing.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Pricing Section -->
  <section class="py-24 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="text-center mb-16">
        <h2 class="text-4xl md:text-5xl font-medium text-gray-900 mb-6 tracking-tight">Simple, Transparent Pricing</h2>
        <p class="text-gray-600 text-lg max-w-2xl mx-auto">Professional coaching costs $120+/hr. CasePrepared gives you 24/7 practice for a fraction of the price.</p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <!-- Free -->
        <div class="bg-white border border-gray-100 rounded-[32px] p-8 shadow-sm flex flex-col">
          <div class="mb-8">
            <h3 class="text-xl font-medium text-gray-900 mb-2">Free</h3>
            <div class="text-4xl font-bold text-gray-900 mb-4">$0</div>
            <p class="text-gray-500 text-sm">Test the system and start practicing.</p>
          </div>
          <ul class="space-y-4 mb-10 flex-grow">
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              3 Case Interviews
            </li>
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              Basic Practice Experience
            </li>
          </ul>
          <a href="#" class="w-full py-3 rounded-full border border-gray-200 text-center font-medium hover:bg-gray-50 transition-colors">Get Started</a>
        </div>

        <!-- Premium -->
        <div class="bg-white border-2 border-[#1e40af] rounded-[32px] p-8 shadow-xl flex flex-col relative transform md:scale-105 z-10">
          <div class="absolute top-0 left-1/2 -translate-x-1/2 -translate-y-1/2 bg-[#1e40af] text-white text-xs font-bold px-4 py-1 rounded-full uppercase tracking-widest">Most Popular</div>
          <div class="mb-8">
            <h3 class="text-xl font-medium text-gray-900 mb-2">Premium</h3>
            <div class="text-4xl font-bold text-gray-900 mb-4">$26.99<span class="text-lg font-normal text-gray-500">/mo</span></div>
            <p class="text-gray-500 text-sm">Serious prep for serious candidates.</p>
          </div>
          <ul class="space-y-4 mb-10 flex-grow">
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              10 Case Interviews
            </li>
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              Post-Interview Feedback
            </li>
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              24/7 Support
            </li>
          </ul>
          <a href="#" class="w-full py-3 rounded-full bg-[#1e40af] text-white text-center font-medium hover:opacity-90 transition-colors">Start Premium</a>
        </div>

        <!-- Pro -->
        <div class="bg-white border border-gray-100 rounded-[32px] p-8 shadow-sm flex flex-col">
          <div class="mb-8">
            <h3 class="text-xl font-medium text-gray-900 mb-2">Pro</h3>
            <div class="text-4xl font-bold text-gray-900 mb-4">$39.99<span class="text-lg font-normal text-gray-500 text-red-500 line-through ml-2">$59.99</span></div>
            <p class="text-gray-500 text-sm">Everything you need to land the offer.</p>
          </div>
          <ul class="space-y-4 mb-10 flex-grow">
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              25+ Case Interviews
            </li>
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              Detailed Analytics
            </li>
            <li class="flex items-center gap-3 text-sm text-gray-600">
              <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/></svg>
              Priority Support
            </li>
          </ul>
          <a href="#" class="w-full py-3 rounded-full border border-gray-200 text-center font-medium hover:bg-gray-50 transition-colors">Go Pro</a>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section class="py-32 px-6 text-center bg-[#1e40af] text-white">
    <div class="max-w-[1200px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-medium mb-6 tracking-tight">
        Ready to land your dream offer?
      </h2>
      <p class="text-blue-100 text-lg max-w-2xl mx-auto mb-10">
        Join students from Harvard, Stanford, and Oxford who are already using CasePrepared to ace their interviews.
      </p>
      <a href="#" class="inline-block bg-white text-[#1e40af] px-8 py-3 rounded-full font-medium transition-colors hover:bg-blue-50">
        Start Practicing Now
      </a>
      <p class="mt-6 text-sm text-blue-200">Secure payments via Stripe</p>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1200px] mx-auto">
      <div class="grid grid-cols-2 md:grid-cols-6 gap-12 mb-20">
        <div class="col-span-2">
          <a href="/" class="flex items-center gap-2 text-[#1e40af] mb-6">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM12 20C7.59 20 4 16.41 4 12C4 7.59 7.59 4 12 4C16.41 4 20 7.59 20 12C20 16.41 16.41 20 12 20Z" fill="currentColor" opacity="0.2"/>
                <path d="M12 6C8.69 6 6 8.69 6 12C6 15.31 8.69 18 12 18C15.31 18 18 15.31 18 12C18 15.31 18 12 12 6ZM12 16C9.79 16 8 14.21 8 12C8 9.79 9.79 8 12 8C14.21 8 16 9.79 16 12C16 14.21 14.21 16 12 16Z" fill="currentColor"/>
            </svg>
            <span class="font-semibold text-lg tracking-widest">CASEPREPARED</span>
          </a>
          <p class="text-sm text-gray-500 max-w-xs">Stronger consulting interview performance via adaptive voice AI simulations.</p>
        </div>
        
        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Product</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Case Library</a></li>
            <li><a href="#" class="hover:text-gray-900">AI Interviewer</a></li>
            <li><a href="#" class="hover:text-gray-900">Analytics</a></li>
            <li><a href="#" class="hover:text-gray-900">Pricing</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Resources</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Blog</a></li>
            <li><a href="#" class="hover:text-gray-900">Case Prep Guide</a></li>
            <li><a href="#" class="hover:text-gray-900">University Program</a></li>
            <li><a href="#" class="hover:text-gray-900">Support</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Company</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">About Us</a></li>
            <li><a href="#" class="hover:text-gray-900">A Pavlos Company</a></li>
            <li><a href="#" class="hover:text-gray-900">Careers</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Legal</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Privacy Policy</a></li>
            <li><a href="#" class="hover:text-gray-900">Terms of Service</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-center pt-8 border-t border-gray-100">
        <div class="text-xs text-gray-500 mb-4 md:mb-0">
          © 2025 CasePrepared. All rights reserved. Part of A Pavlos Company.
        </div>

        <div class="flex items-center gap-4 text-gray-400">
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg></a>
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg></a>
        </div>
      </div>
    </div>
  </footer>
</div>



