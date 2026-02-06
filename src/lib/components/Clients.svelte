<script lang="ts">
  const partners = [
    { name: "Ministry of Defense of Ukraine", logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/0/0d/Emblem_of_the_Ministry_of_Defence_of_Ukraine.svg/1200px-Emblem_of_the_Ministry_of_Defence_of_Ukraine.svg.png" },
    { name: "Ministry of Digital Transformation", logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/5f/Ministry_of_Digital_Transformation_of_Ukraine.svg/1200px-Ministry_of_Digital_Transformation_of_Ukraine.svg.png" },
    { name: "United24", logo: "" },
    { name: "Unmanned Systems Forces", logo: "" }
  ];
</script>

<section class="bg-white text-gray-900 py-24 px-6 md:px-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="mb-12 border-b border-gray-200 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">Strategic Partners & Government Relations</span>
    </div>

    <!-- Headline -->
    <h2 class="text-3xl md:text-4xl font-light leading-tight mb-16 max-w-3xl">
      Trusted by governments and defense forces — 
      <span class="font-serif italic text-gray-400">working directly with the infrastructure of modern defense.</span>
    </h2>

    <!-- Logos Grid -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-px bg-gray-200 border border-gray-200">
      <!-- Partner 1: MoD Ukraine -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="h-32 w-32 relative mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-full h-full">
              <circle cx="50" cy="50" r="45" stroke="black" stroke-width="2"/>
              <path d="M50 15V85M15 50H85" stroke="black" stroke-width="2"/>
              <path d="M30 30L70 70M70 30L30 70" stroke="black" stroke-width="2"/>
            </svg>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Ministry of Defense of Ukraine</span>
      </div>

      <!-- Partner 2: MoDT Ukraine -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="flex items-center gap-4 mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <div class="text-4xl font-bold tracking-tighter">ДІЯ</div>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Ministry of Digital Transformation</span>
      </div>

      <!-- Partner 3: United24 -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="flex items-center gap-3 mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <span class="text-3xl font-bold tracking-widest uppercase text-gray-900">UNITED24</span>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Government Initiative</span>
      </div>

      <!-- Partner 4: USF -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="flex flex-col items-center mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <svg width="60" height="60" viewBox="0 0 60 60" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M10 50L30 10L50 50H10Z" stroke="black" stroke-width="3"/>
              <circle cx="30" cy="35" r="5" fill="black"/>
            </svg>
            <span class="text-xl font-bold uppercase tracking-widest mt-2">USF</span>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Unmanned Systems Forces</span>
      </div>
    </div>
  </div>
</section>