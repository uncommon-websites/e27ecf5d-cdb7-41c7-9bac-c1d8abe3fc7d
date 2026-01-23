<script lang="ts">
  import Logo from './Logo.svelte';
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-white/95 backdrop-blur-lg border-b border-gray-100">
  <!-- Announcement Bar -->
  <div class="w-full py-2.5 text-center bg-gradient-to-r from-blue-600 to-cyan-600 hidden md:block">
    <a href="#" class="text-sm font-semibold text-white hover:text-white/90 transition-colors">
      Custom AI solutions for your business
    </a>
  </div>

  <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
    <!-- Logo -->
    <div class="flex-shrink-0">
      <a href="/" class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-blue-600 to-cyan-600 flex items-center justify-center">
          <Logo className="w-5 h-5 text-white" />
        </div>
        <span class="font-bold text-xl text-gray-900">AI Studio</span>
      </a>
    </div>

    <!-- Navigation -->
    <div class="hidden md:flex items-center gap-8 text-base font-medium text-gray-600">
      <a href="#" class="hover:text-blue-600 transition-colors">Services</a>
      <a href="#" class="hover:text-blue-600 transition-colors">Case studies</a>
      <a href="#" class="hover:text-blue-600 transition-colors">Our team</a>
      <a href="#" class="hover:text-blue-600 transition-colors">Contact</a>
    </div>

    <!-- Actions -->
    <div class="flex items-center gap-4">
      <a href="#" class="text-gray-600 hover:text-gray-900 font-medium transition-colors hidden sm:block">About us</a>
      <a href="#" class="bg-gradient-to-r from-blue-600 to-cyan-600 hover:from-blue-700 hover:to-cyan-700 text-white px-6 py-3 rounded-full transition-all font-bold shadow-lg hover:shadow-xl hover:scale-105">
        Start your project
      </a>
    </div>
  </div>
</nav>
