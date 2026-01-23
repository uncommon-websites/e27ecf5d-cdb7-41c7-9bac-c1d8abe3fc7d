<script lang="ts">
  import Navbar from '$lib/components/Navbar.svelte';

  const universityLogos = [
    "Harvard", "Stanford", "Wharton", "Oxford", "Penn", "IE", "Bocconi", "Dartmouth"
  ];

  const features = [
    {
      icon: "microphone",
      title: "Voice AI Interviews",
      description: "Practice with an AI that sounds and responds like a real McKinsey partner"
    },
    {
      icon: "chart",
      title: "Performance Analytics",
      description: "Get detailed feedback on structure, logic, communication, and insights"
    },
    {
      icon: "library",
      title: "Full Case Library",
      description: "25+ cases covering M&A, market entry, pricing, growth, and more"
    },
    {
      icon: "adaptive",
      title: "Adaptive Difficulty",
      description: "AI adjusts complexity based on your performance in real-time"
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
          <span class="text-sm font-semibold text-blue-700">Trusted by Harvard, Stanford, Wharton students</span>
        </div>
        
        <h1 class="text-5xl md:text-7xl lg:text-8xl font-bold mb-8 leading-[1.1]">
          Master consulting<br>
          <span class="text-gradient">interviews with AI</span>
        </h1>
        
        <p class="text-xl md:text-2xl text-gray-600 max-w-3xl mx-auto mb-12 leading-relaxed">
          Practice with realistic voice AI simulations and get detailed analytics to land your dream offer at McKinsey, BCG, or Bain.
        </p>
        
        <!-- CTA Buttons -->
        <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-16">
          <a href="#" class="group relative inline-flex items-center gap-2 bg-gradient-to-r from-blue-600 to-cyan-600 text-white px-8 py-4 rounded-full font-bold text-lg transition-all hover:scale-105 hover:shadow-2xl glow-blue">
            Start practicing free
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" class="group-hover:translate-x-1 transition-transform"><path d="m9 18 6-6-6-6"/></svg>
          </a>
          <a href="#" class="inline-flex items-center gap-2 bg-white border-2 border-gray-200 text-gray-900 px-8 py-4 rounded-full font-bold text-lg transition-all hover:border-blue-300 hover:bg-blue-50">
            View pricing
          </a>
        </div>
      </div>

      <!-- Hero Cards -->
      <div class="grid md:grid-cols-3 gap-6 max-w-6xl mx-auto">
        <!-- Card 1 -->
        <div class="card-gradient-1 rounded-3xl p-8 text-white transform hover:scale-105 transition-all glow-blue">
          <div class="w-12 h-12 bg-white/20 rounded-2xl flex items-center justify-center mb-6 backdrop-blur-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" y1="19" x2="12" y2="23"/><line x1="8" y1="23" x2="16" y2="23"/></svg>
          </div>
          <h3 class="text-2xl font-bold mb-3">Voice AI</h3>
          <p class="text-white/90 leading-relaxed">Speak naturally with an AI interviewer that adapts to your responses</p>
        </div>

        <!-- Card 2 -->
        <div class="card-gradient-2 rounded-3xl p-8 text-white transform hover:scale-105 transition-all">
          <div class="w-12 h-12 bg-white/20 rounded-2xl flex items-center justify-center mb-6 backdrop-blur-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21.21 15.89A10 10 0 1 1 8 2.83"/><path d="M22 12A10 10 0 0 0 12 2v10z"/></svg>
          </div>
          <h3 class="text-2xl font-bold mb-3">Deep Analytics</h3>
          <p class="text-white/90 leading-relaxed">Get detailed feedback on structure, logic, and communication</p>
        </div>

        <!-- Card 3 -->
        <div class="card-gradient-3 rounded-3xl p-8 text-white transform hover:scale-105 transition-all glow-cyan">
          <div class="w-12 h-12 bg-white/20 rounded-2xl flex items-center justify-center mb-6 backdrop-blur-sm">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>
          </div>
          <h3 class="text-2xl font-bold mb-3">25+ Cases</h3>
          <p class="text-white/90 leading-relaxed">Practice every case type from market entry to M&A</p>
        </div>
      </div>
    </div>
  </main>

  <!-- Logos Section -->
  <section class="py-20 bg-gray-50">
    <div class="max-w-7xl mx-auto px-6">
      <p class="text-center text-sm text-gray-500 mb-12 uppercase tracking-wider font-bold">Trusted by students at</p>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-8 items-center justify-items-center">
        {#each universityLogos as university}
          <div class="h-10 flex items-center">
            <span class="font-bold text-2xl text-gray-400 hover:text-blue-600 transition-colors">{university}</span>
          </div>
        {/each}
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
            Voice AI Technology
          </div>
          
          <h2 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
            Practice like you're in the real interview
          </h2>
          
          <p class="text-xl text-gray-600 mb-10 leading-relaxed">
            Our AI interviewer sounds, thinks, and responds like a real McKinsey partner. No static prompts—just natural conversation.
          </p>

          <div class="space-y-6">
            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" y1="19" x2="12" y2="23"/><line x1="8" y1="23" x2="16" y2="23"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Natural voice interaction</h3>
                <p class="text-gray-600 leading-relaxed">
                  Speak naturally and get intelligent follow-up questions based on your responses
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-cyan-500 to-teal-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Adaptive difficulty</h3>
                <p class="text-gray-600 leading-relaxed">
                  AI adjusts complexity in real-time based on your performance level
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-indigo-500 to-blue-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Complete case library</h3>
                <p class="text-gray-600 leading-relaxed">
                  25+ cases covering M&A, market entry, pricing, growth, and operations
                </p>
              </div>
            </div>
          </div>
        </div>

        <!-- Visual -->
        <div class="relative">
          <div class="absolute inset-0 bg-gradient-to-br from-blue-500 to-cyan-500 rounded-3xl blur-3xl opacity-20"></div>
          <div class="relative bg-white rounded-3xl p-8 border-2 border-gray-100 shadow-2xl">
            <img src="/generated/image-a-student-in-a-modern-library-using-a-la-1769124077989-0.webp" alt="Student practicing case" class="w-full h-full object-cover rounded-2xl" />
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial Section -->
  <section class="py-20 px-6 bg-gradient-to-br from-blue-50 to-cyan-50">
    <div class="max-w-5xl mx-auto">
      <div class="bg-white rounded-3xl p-10 md:p-16 shadow-2xl border-2 border-blue-100 relative overflow-hidden">
        <div class="absolute top-0 right-0 w-64 h-64 bg-gradient-to-br from-blue-500 to-cyan-500 rounded-full blur-3xl opacity-10"></div>
        
        <div class="relative z-10">
          <div class="flex items-center gap-3 mb-8">
            <div class="flex gap-1">
              {#each Array(5) as _}
                <svg class="w-6 h-6 text-yellow-400" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
              {/each}
            </div>
            <span class="text-sm font-bold text-blue-600 uppercase tracking-wider">Wharton MBA</span>
          </div>
          
          <blockquote class="text-3xl md:text-4xl font-bold leading-tight text-gray-900 mb-10">
            "CasePrepared is a game-changer. The AI's ability to probe my logic is as close to a real coach as it gets, but at a fraction of the cost."
          </blockquote>
          
          <div class="flex items-center gap-4">
            <img src="https://i.pravatar.cc/100?img=12" alt="Candidate" class="w-16 h-16 rounded-full object-cover border-4 border-blue-100" />
            <div>
              <div class="font-bold text-lg text-gray-900">Alex Chen</div>
              <div class="text-gray-600">Incoming Associate at MBB</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 2 (Analytics) -->
  <section class="py-32 px-6 bg-white">
    <div class="max-w-7xl mx-auto">
      <div class="grid md:grid-cols-2 gap-16 items-center">
        <!-- Visual -->
        <div class="relative order-2 md:order-1">
          <div class="absolute inset-0 bg-gradient-to-br from-cyan-500 to-emerald-500 rounded-3xl blur-3xl opacity-20"></div>
          <div class="relative bg-white rounded-3xl p-8 border-2 border-gray-100 shadow-2xl">
            <img src="/generated/image-a-close-up-of-a-tablet-screen-showing-de-1769124080812-1.webp" alt="Analytics Dashboard" class="w-full h-full object-cover rounded-2xl" />
          </div>
        </div>

        <!-- Content -->
        <div class="order-1 md:order-2">
          <div class="inline-block bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm font-bold mb-6">
            Performance Analytics
          </div>
          
          <h2 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
            Get feedback that actually helps you improve
          </h2>
          
          <p class="text-xl text-gray-600 mb-10 leading-relaxed">
            Our AI analyzes every aspect of your performance and gives you actionable insights to level up your interview skills.
          </p>

          <div class="space-y-6">
            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21.21 15.89A10 10 0 1 1 8 2.83"/><path d="M22 12A10 10 0 0 0 12 2v10z"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Logic and structure scoring</h3>
                <p class="text-gray-600 leading-relaxed">
                  Detailed breakdown of your frameworks, math accuracy, and insight quality
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-cyan-500 to-teal-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Communication analysis</h3>
                <p class="text-gray-600 leading-relaxed">
                  Track filler words, pace, thinking time, and tone to sound confident
                </p>
              </div>
            </div>

            <div class="flex gap-4 items-start">
              <div class="w-12 h-12 rounded-2xl bg-gradient-to-br from-indigo-500 to-blue-500 flex items-center justify-center flex-shrink-0">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
              </div>
              <div>
                <h3 class="font-bold text-lg text-gray-900 mb-2">Full transcript review</h3>
                <p class="text-gray-600 leading-relaxed">
                  See exactly what you said with suggestions for better phrasing
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Pricing Section -->
  <section class="py-32 px-6 bg-gray-50">
    <div class="max-w-7xl mx-auto">
      <div class="text-center mb-20">
        <div class="inline-block bg-blue-100 text-blue-700 px-4 py-2 rounded-full text-sm font-bold mb-6">
          Pricing
        </div>
        <h2 class="text-4xl md:text-6xl font-bold mb-6">Choose your plan</h2>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto">Professional coaching costs $120+/hour. Get 24/7 AI practice for a fraction of the price.</p>
      </div>

      <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
        <!-- Free -->
        <div class="bg-white rounded-3xl p-8 border-2 border-gray-200 flex flex-col hover:border-blue-300 transition-all">
          <div class="mb-8">
            <h3 class="text-2xl font-bold text-gray-900 mb-4">Free</h3>
            <div class="flex items-baseline gap-2 mb-4">
              <span class="text-5xl font-bold text-gray-900">$0</span>
            </div>
            <p class="text-gray-600">Test the platform and start practicing</p>
          </div>
          <ul class="space-y-4 mb-10 flex-grow">
            <li class="flex items-center gap-3 text-gray-700">
              <svg class="w-6 h-6 text-emerald-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">3 case interviews</span>
            </li>
            <li class="flex items-center gap-3 text-gray-700">
              <svg class="w-6 h-6 text-emerald-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">Basic practice experience</span>
            </li>
          </ul>
          <a href="#" class="w-full py-4 rounded-full border-2 border-gray-200 text-center font-bold hover:bg-gray-50 transition-all">Get started</a>
        </div>

        <!-- Premium -->
        <div class="bg-gradient-to-br from-blue-600 to-cyan-600 rounded-3xl p-8 flex flex-col relative transform md:scale-105 shadow-2xl glow-blue">
          <div class="absolute -top-4 left-1/2 -translate-x-1/2 bg-indigo-500 text-white text-xs font-bold px-6 py-2 rounded-full uppercase tracking-wider shadow-lg">
            Most Popular
          </div>
          <div class="mb-8">
            <h3 class="text-2xl font-bold text-white mb-4">Premium</h3>
            <div class="flex items-baseline gap-2 mb-4">
              <span class="text-5xl font-bold text-white">$27</span>
              <span class="text-xl text-white/80">/month</span>
            </div>
            <p class="text-white/90">Serious prep for serious candidates</p>
          </div>
          <ul class="space-y-4 mb-10 flex-grow">
            <li class="flex items-center gap-3 text-white">
              <svg class="w-6 h-6 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">10 case interviews</span>
            </li>
            <li class="flex items-center gap-3 text-white">
              <svg class="w-6 h-6 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">Post-interview feedback</span>
            </li>
            <li class="flex items-center gap-3 text-white">
              <svg class="w-6 h-6 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">24/7 support</span>
            </li>
          </ul>
          <a href="#" class="w-full py-4 rounded-full bg-white text-blue-600 text-center font-bold hover:bg-gray-50 transition-all shadow-lg">Start premium</a>
        </div>

        <!-- Pro -->
        <div class="bg-white rounded-3xl p-8 border-2 border-gray-200 flex flex-col hover:border-blue-300 transition-all">
          <div class="mb-8">
            <h3 class="text-2xl font-bold text-gray-900 mb-4">Pro</h3>
            <div class="flex items-baseline gap-2 mb-4">
              <span class="text-5xl font-bold text-gray-900">$40</span>
              <span class="text-xl text-gray-500 line-through">$60</span>
            </div>
            <p class="text-gray-600">Everything you need to land the offer</p>
          </div>
          <ul class="space-y-4 mb-10 flex-grow">
            <li class="flex items-center gap-3 text-gray-700">
              <svg class="w-6 h-6 text-emerald-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">25+ case interviews</span>
            </li>
            <li class="flex items-center gap-3 text-gray-700">
              <svg class="w-6 h-6 text-emerald-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">Detailed analytics</span>
            </li>
            <li class="flex items-center gap-3 text-gray-700">
              <svg class="w-6 h-6 text-emerald-500 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"/></svg>
              <span class="font-medium">Priority support</span>
            </li>
          </ul>
          <a href="#" class="w-full py-4 rounded-full border-2 border-gray-900 bg-gray-900 text-white text-center font-bold hover:bg-gray-800 transition-all">Go pro</a>
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
        Ready to ace your<br>consulting interviews?
      </h2>
      <p class="text-xl md:text-2xl text-white/90 max-w-2xl mx-auto mb-12 leading-relaxed">
        Join students from Harvard, Stanford, and Wharton who are already using CasePrepared to land their dream offers.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <a href="#" class="group inline-flex items-center gap-2 bg-white text-blue-600 px-10 py-5 rounded-full font-bold text-lg transition-all hover:scale-105 shadow-2xl">
          Start practicing free
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" class="group-hover:translate-x-1 transition-transform"><path d="m9 18 6-6-6-6"/></svg>
        </a>
        <a href="#" class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm border-2 border-white/30 text-white px-10 py-5 rounded-full font-bold text-lg transition-all hover:bg-white/20">
          View pricing
        </a>
      </div>
      <p class="mt-8 text-white/80 text-sm">Secure payments via Stripe • No credit card required for free plan</p>
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
            <span class="font-bold text-xl tracking-tight">CasePrepared</span>
          </a>
          <p class="text-gray-400 max-w-xs leading-relaxed">Master consulting interviews with adaptive voice AI simulations and detailed analytics.</p>
        </div>
        
        <div>
          <h4 class="font-bold text-white mb-4">Product</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">Case library</a></li>
            <li><a href="#" class="hover:text-white transition-colors">AI interviewer</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Analytics</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Pricing</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-bold text-white mb-4">Resources</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">Blog</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Case prep guide</a></li>
            <li><a href="#" class="hover:text-white transition-colors">University program</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Support</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-bold text-white mb-4">Company</h4>
          <ul class="space-y-3 text-gray-400">
            <li><a href="#" class="hover:text-white transition-colors">About us</a></li>
            <li><a href="#" class="hover:text-white transition-colors">A Pavlos Company</a></li>
            <li><a href="#" class="hover:text-white transition-colors">Careers</a></li>
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
          © 2025 CasePrepared. All rights reserved. Part of A Pavlos Company.
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



