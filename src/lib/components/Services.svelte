<script lang="ts">
  const capabilities = [
    {
      title: "M4 Ground Robot",
      description: "A versatile 4x4 electric robot with 25 km/h speed, 15 kg payload, and 20+ km effective range. Portable and battle-ready.",
      image: "/generated/image-a-sophisticated-autonomous-ground-robot--1770410408804-0.webp"
    },
    {
      title: "Remote Operations",
      description: "Control drones and robots from 2,000 kilometers away with video-game-like interfaces for robotic swarms.",
      image: "/generated/image-a-close-up-of-a-ruggedized-tablet-interf-1770410421601-3.webp"
    },
    {
      title: "Collaborative Autonomy",
      description: "Real-time mission execution across distributed fleets. Scalable from single units to thousands of coordinated robots.",
      image: "https://images.unsplash.com/photo-1485827404703-89b55fcc595e?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Security Architecture",
      description: "Defense-grade autonomy with layered security and secure communication protocols. System-agnostic operation.",
      image: "https://images.unsplash.com/photo-1550751827-4bd374c3f58b?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Mission Planning",
      description: "Integration of waypoint-based mission planning with live battlespace mapping for real-time tactical advantage.",
      image: "https://images.unsplash.com/photo-1581092160562-40aa08e78837?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Robot Family (A1, M4, X1)",
      description: "A suite of models designed to accelerate collaborative autonomy development and deployment across various environments.",
      image: "https://images.unsplash.com/photo-1531746790731-6c087fecd05a?q=80&w=1000&auto=format&fit=crop"
    }
  ];
</script>

<section id="system" class="bg-white text-gray-900 py-24 px-6 md:px-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="mb-12 border-b border-gray-200 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">Technical Capabilities & Product Ecosystem</span>
    </div>

    <!-- Main Headline -->
    <h2 class="text-4xl md:text-5xl lg:text-5xl font-light leading-tight mb-24 max-w-4xl">
      From single units to coordinated fleets, we provide the 
      <span class="font-serif italic">full-stack command and control</span> 
      systems for modern defense forces.
    </h2>

    <!-- Services List -->
    <div class="space-y-24">
      {#each capabilities as service, i}
        <div class="group grid grid-cols-1 md:grid-cols-12 gap-8 items-center border-b border-gray-100 pb-24 last:border-0 last:pb-0">
          
          <!-- Image (Alternating) -->
          <div class="md:col-span-5 {i % 2 === 1 ? 'md:order-last' : ''}">
            <div class="aspect-[16/9] overflow-hidden bg-gray-100 relative">
               <img src={service.image} alt={service.title} class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
            </div>
          </div>

          <!-- Content -->
          <div class="md:col-span-7 {i % 2 === 1 ? 'md:pr-12 md:text-right flex flex-col items-end' : 'md:pl-12'}">
             <h3 class="text-3xl font-light mb-6 group-hover:text-primary-500 transition-colors">{service.title}</h3>
             <p class="text-gray-500 font-light leading-relaxed max-w-md mb-8 {i % 2 === 1 ? 'text-right' : ''}">
               {service.description}
             </p>
             
             <a href="#missions" class="inline-flex items-center gap-2 px-6 py-2 bg-primary-100 rounded-full text-[10px] font-bold uppercase tracking-wider hover:bg-primary-500 hover:text-white transition-colors duration-300 text-primary-900">
                View Missions
                <svg width="8" height="8" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="rotate-45">
                  <path d="M7 17L17 7M17 7H7M17 7V17" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </a>
          </div>

        </div>
      {/each}
    </div>
  </div>
</section>