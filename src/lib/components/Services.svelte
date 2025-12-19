<script lang="ts">
  const services = [
    {
      title: "Design Consultation",
      description: "They help quickly validate existing ideas for developing green spaces or create new concepts from scratch.",
      image: "https://images.unsplash.com/photo-1600607686527-6fb886090705?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Concept for Green Area",
      description: "A functional layout reflecting the style (plantings, hard paths, stones, etc.) tailored to the client's needs.",
      image: "https://images.unsplash.com/photo-1557429287-b2e26467fc2b?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Plant Composition",
      description: "Arrangement of planting beds, lawns, hedges, planters, etc., as well as selection of specific plant species.",
      image: "https://images.unsplash.com/photo-1613977257363-707ba9348227?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Concept Plan for Green",
      description: "Serves as the primary documentation for implementation. Its exact scope is determined individually.",
      image: "https://images.unsplash.com/photo-1585320806297-9794b3e4eeae?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Supervision Over an Implementation",
      description: "Recommending specialists for sourcing local stones and bonsai plants, supervising on-site implementation for design compliance, and maintaining ongoing communication with the investor and contractors.",
      image: "https://images.unsplash.com/photo-1591825729269-caeb344f6df2?q=80&w=1000&auto=format&fit=crop"
    },
    {
      title: "Gardening Workshops",
      description: "Conducting workshops in the form of planting events, joint gardening activities, or nature walks for organized groups or open neighborhood events.",
      image: "https://images.unsplash.com/photo-1416879595882-3373a0480b5b?q=80&w=1000&auto=format&fit=crop"
    }
  ];
</script>

<section class="bg-white text-gray-900 py-24 px-6 md:px-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="mb-12 border-b border-gray-200 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">Tailored Offer to Meet Your Needs</span>
    </div>

    <!-- Main Headline -->
    <h2 class="text-4xl md:text-5xl lg:text-5xl font-light leading-tight mb-24 max-w-4xl">
      From concept to completion, I offer a full range of landscape design services to 
      <span class="font-serif italic">transform outdoor spaces into beautiful</span>, 
      and functional environments.
    </h2>

    <!-- Services List -->
    <div class="space-y-24">
      {#each services as service, i}
        <div class="group grid grid-cols-1 md:grid-cols-12 gap-8 items-center border-b border-gray-100 pb-24 last:border-0 last:pb-0">
          
          <!-- Image (Alternating) -->
          <div class="md:col-span-5 {i % 2 === 1 ? 'md:order-last' : ''}">
            <div class="aspect-[16/9] overflow-hidden bg-gray-100 relative">
               <img src={service.image} alt={service.title} class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105" />
            </div>
          </div>

          <!-- Content -->
          <div class="md:col-span-7 {i % 2 === 1 ? 'md:pr-12 md:text-right flex flex-col items-end' : 'md:pl-12'}">
             <h3 class="text-3xl font-light mb-6 group-hover:text-dark-green transition-colors">{service.title}</h3>
             <p class="text-gray-500 font-light leading-relaxed max-w-md mb-8 {i % 2 === 1 ? 'text-right' : ''}">
               {service.description}
             </p>
             
             <a href="/services" class="inline-flex items-center gap-2 px-6 py-2 bg-lime-green/50 rounded-full text-[10px] font-bold uppercase tracking-wider hover:bg-lime-green transition-colors duration-300 text-dark-green">
                More
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