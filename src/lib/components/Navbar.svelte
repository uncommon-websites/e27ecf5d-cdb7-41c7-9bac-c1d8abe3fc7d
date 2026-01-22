<script>
  import Logo from './Logo.svelte';
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm transition-all duration-300 border-b border-gray-100/50">
  <!-- Announcement Bar -->
  <div class="w-full py-2 text-center bg-[#f7f7f7] border-b border-transparent hidden md:block">
    <a href="#" class="text-[11px] font-medium text-[#334155] hover:text-gray-900 underline underline-offset-2 transition-colors">
      Book an AI demo for your University.
    </a>
  </div>

  <div class="max-w-[1400px] mx-auto px-6 h-20 flex items-center justify-between">
    <!-- Logo -->
    <div class="flex-shrink-0">
      <a href="/" class="flex items-center gap-2 text-[#1e40af]">
        <Logo className="w-7 h-7" />
        <span class="font-semibold text-lg tracking-widest text-[#1e40af]">CASEPREPARED</span>
      </a>
    </div>

    <!-- Navigation -->
    <div class="hidden md:flex items-center gap-10 text-[15px] font-normal text-[#334155]">
      <a href="#" class="hover:text-gray-900 transition-colors">Pricing</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Case Library</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Resources</a>
      <a href="#" class="hover:text-gray-900 transition-colors">University</a>
    </div>

    <!-- Actions -->
    <div class="flex items-center gap-6 text-[15px] font-normal">
      <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors hidden sm:block">Sign in</a>
      <a href="#" class="bg-[#1e40af] hover:opacity-90 text-white px-5 py-2.5 rounded-full transition-colors font-medium">
        Start practicing
      </a>
    </div>
  </div>
</nav>
