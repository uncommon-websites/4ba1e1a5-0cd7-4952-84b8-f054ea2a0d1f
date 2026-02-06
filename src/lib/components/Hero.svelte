<script lang="ts">
  import { onMount } from 'svelte';
</script>

<section class="h-screen w-full overflow-hidden relative flex flex-col bg-dark-green text-pale-green">
    <!-- Background Placeholder (Simulating the video noise/texture mentioned in screenshot) -->
    <div class="absolute inset-0 w-full h-full -z-10 opacity-30 pointer-events-none" style="background: radial-gradient(circle at 50% 50%, #440000 0%, #220101 100%);"></div>

    <!-- Main Hero Content -->
    <main class="flex-grow flex flex-col items-center justify-center relative z-10 -mt-10">
        
        <!-- Center Typography -->
        <div class="text-center">
            <!-- Line 1: Mixed Serif & Italic -->
            <h1 class="text-5xl md:text-7xl lg:text-[7.5rem] leading-[0.9] text-pale-green whitespace-nowrap">
                <span class="font-serif font-normal">Networked</span>
                <span class="font-serif italic font-normal ml-2 md:ml-4">Autonomy</span>
                <span class="font-thin mx-2 md:mx-6 opacity-80">—</span>
                <span class="font-serif italic font-normal">Fleets</span>
            </h1>
            
            <!-- Line 2: Sans Serif -->
            <h2 class="text-5xl md:text-7xl lg:text-[7.5rem] leading-[0.9] font-normal mt-2 md:mt-4 text-pale-green">
                Deploying at Mission Scale.
            </h2>
        </div>

        <!-- Floating Elements -->
        
        <!-- Left Floating Text -->
        <div class="absolute left-[15%] top-[65%] hidden lg:block">
            <span class="text-[10px] font-bold tracking-[0.2em] uppercase opacity-90">(Battlefield Proven)</span>
        </div>

        <!-- Right Floating Text -->
        <div class="absolute right-[12%] top-[65%] max-w-[280px] hidden lg:block text-left">
            <p class="text-xl font-light leading-relaxed opacity-90">
                Connecting autonomous robots into collaborative fleets via networked infrastructure.
            </p>
        </div>

        <!-- "Video noise" placeholder elements -->
        <div class="absolute bottom-32 left-8 flex items-center gap-2 opacity-50 text-xs">
            <div class="w-4 h-4 rounded-sm bg-pale-green/20 flex items-center justify-center text-[10px]">+</div>
            <span>Video noise</span>
        </div>

    </main>

    <!-- Bottom Navigation & Controls -->
    <div class="absolute bottom-8 left-0 w-full px-8 flex justify-between items-end z-20">
        
        <!-- Left: Inquiry Button -->
        <button class="bg-pale-green text-dark-green px-6 py-3 rounded-full flex items-center gap-2 text-xs font-bold tracking-wide hover:bg-white transition-colors group">
            REQUEST DEPLOYMENT
            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="group-hover:translate-x-0.5 group-hover:-translate-y-0.5 transition-transform">
                <line x1="7" y1="17" x2="17" y2="7"></line>
                <polyline points="7 7 17 7 17 17"></polyline>
            </svg>
        </button>

        <!-- Center: Navigation Pills -->
        <nav class="bg-nav-pill p-1.5 rounded-full flex gap-1 absolute left-1/2 transform -translate-x-1/2 shadow-lg">
            <a href="/" class="bg-pale-green text-dark-green px-6 py-2.5 rounded-full text-xs font-bold tracking-wide">
                HOME
            </a>
            <a href="#platform" class="text-pale-green px-6 py-2.5 rounded-full text-xs font-bold tracking-wide hover:bg-white/5 transition-colors">
                PLATFORM
            </a>
            <a href="#missions" class="text-pale-green px-6 py-2.5 rounded-full text-xs font-bold tracking-wide hover:bg-white/5 transition-colors">
                MISSIONS
            </a>
            <a href="#system" class="text-pale-green px-6 py-2.5 rounded-full text-xs font-bold tracking-wide hover:bg-white/5 transition-colors">
                SYSTEM
            </a>
        </nav>

        <!-- Right: Cookies & Scroll -->
        <div class="flex items-center gap-6">
            <!-- Cookie Banner -->
            <div class="flex items-center gap-4 bg-transparent">
                <span class="text-sm font-medium opacity-90 hidden md:inline">Autonomous systems data active</span>
                <button class="bg-white text-dark-green px-5 py-2 rounded-full text-xs font-bold hover:bg-gray-200 transition-colors">
                    Accept
                </button>
            </div>

            <!-- Scroll Down Button -->
            <button class="bg-pale-green text-dark-green w-12 h-12 rounded-full flex items-center justify-center hover:bg-white transition-colors hover:scale-105 transform duration-200">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <line x1="12" y1="5" x2="12" y2="19"></line>
                    <polyline points="19 12 12 19 5 12"></polyline>
                </svg>
            </button>
        </div>
    </div>
</section>