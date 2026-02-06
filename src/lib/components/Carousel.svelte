<script lang="ts">
  const segments = [
    {
      id: "01",
      title: "Governments",
      description: "Supporting national defense and security strategies of liberal democracies. Focus on mass robotics integration and autonomous fleet deployment.",
      image: "https://images.unsplash.com/photo-1521791136064-7986c295944b?q=80&w=1000&auto=format&fit=crop"
    },
    {
      id: "02",
      title: "Defense Forces",
      description: "Allied military partnerships, full-stack command and control systems, frontline and border operations, and scale deployment capabilities.",
      image: "/generated/image-a-fleet-of-small-autonomous-drones-flyin-1770410418484-2.webp"
    },
    {
      id: "03",
      title: "Enterprises",
      description: "Farming applications, logistics operations, infrastructure maintenance, and multi-system solutions for competitive advantage.",
      image: "https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?q=80&w=1000&auto=format&fit=crop"
    }
  ];
</script>

<section id="platform" class="bg-dark-green text-pale-green py-24 px-6 md:px-12 overflow-hidden">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="mb-12 border-b border-white/10 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium opacity-60">Strategic Customer Segments & Markets</span>
    </div>

    <!-- Header & Nav -->
    <div class="flex flex-col md:flex-row justify-between items-end mb-20 gap-8">
      <h2 class="text-4xl md:text-5xl font-light leading-tight max-w-3xl">
        Serving a <span class="font-serif italic text-primary-400">diverse range of sectors</span>,
        from national defense to industrial automation — enabling collaborative autonomy at scale.
      </h2>
      
      <div class="flex gap-4">
        <button class="w-12 h-12 rounded-full border border-white/20 flex items-center justify-center hover:bg-white hover:text-dark-green transition-colors">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M19 12H5M5 12L12 19M5 12L12 5" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
        <button class="w-12 h-12 rounded-full border border-white/20 flex items-center justify-center hover:bg-white hover:text-dark-green transition-colors">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M5 12H19M19 12L12 5M19 12L12 19" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
      </div>
    </div>

    <!-- Carousel -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each segments as segment}
        <div class="group relative aspect-[4/5] bg-gray-900 overflow-hidden cursor-pointer">
          <img src={segment.image} alt={segment.title} class="w-full h-full object-cover opacity-60 group-hover:opacity-40 group-hover:scale-105 transition-all duration-700" />
          
          <div class="absolute inset-0 p-8 flex flex-col justify-between">
            <span class="text-xs font-mono opacity-60">({segment.id})</span>
            
            <div class="transform translate-y-4 group-hover:translate-y-0 transition-transform duration-500">
              <h3 class="text-2xl font-light mb-4">{segment.title}</h3>
              <p class="text-sm opacity-0 group-hover:opacity-80 transition-opacity duration-500 delay-100 font-light leading-relaxed">
                {segment.description}
              </p>
            </div>
          </div>
        </div>
      {/each}
    </div>

  </div>
</section>