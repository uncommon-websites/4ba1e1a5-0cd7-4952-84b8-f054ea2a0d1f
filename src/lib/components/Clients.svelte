<script lang="ts">
  const clients = [
    { name: "Powiat Tucholski", logo: "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/POL_powiat_tucholski_COA.svg/1200px-POL_powiat_tucholski_COA.svg.png" },
    { name: "Miasto Września", logo: "https://upload.wikimedia.org/wikipedia/commons/e/e4/POL_Wrze%C5%9Bnia_logo.svg" }, // Placeholder, using text in real impl if logo unavailable
    { name: "Soliddom sp. z o.o.", logo: "" }, // Text based logo
    { name: "LINEA sp. z o.o.", logo: "" } // Text based logo
  ];
</script>

<section class="bg-white text-gray-900 py-24 px-6 md:px-12 border-t border-gray-100">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="mb-12 border-b border-gray-200 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">My Featured Clients</span>
    </div>

    <!-- Headline -->
    <h2 class="text-3xl md:text-4xl font-light leading-tight mb-16 max-w-3xl">
      Trusted by clients who value exceptional design — 
      <span class="font-serif italic text-gray-400">explore some of the brands and individuals I've had the pleasure to work with.</span>
    </h2>

    <!-- Logos Grid -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-px bg-gray-200 border border-gray-200">
      <!-- Client 1: Powiat Tucholski -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="h-32 w-32 relative mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <!-- Simplified Shield SVG -->
            <svg viewBox="0 0 100 120" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-full h-full">
              <path d="M10 10 H90 V60 C90 90 50 110 50 110 C50 110 10 90 10 60 V10 Z" fill="#FFD700" stroke="black" stroke-width="2"/>
              <path d="M20 20 H80 V50" fill="#D22" /> 
              <!-- Eagle shape approximation -->
              <path d="M30 40 L50 30 L70 40 L60 70 L50 90 L40 70 Z" fill="black"/>
            </svg>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Powiat Tucholski</span>
      </div>

      <!-- Client 2: Miasto Września -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="flex items-center gap-4 mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <!-- Flower Symbol -->
            <svg width="60" height="60" viewBox="0 0 60 60" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M30 0L36 24L60 30L36 36L30 60L24 36L0 30L24 24L30 0Z" fill="#8B1A1A"/>
              <circle cx="30" cy="30" r="5" fill="white"/>
            </svg>
            <div class="flex flex-col">
               <span class="text-3xl font-bold tracking-widest uppercase text-gray-900 leading-none">Września</span>
            </div>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Miasto Września</span>
      </div>

      <!-- Client 3: SolidDom -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="flex items-center gap-3 mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
               <path d="M10 10H25V40H10V10Z" fill="black"/>
               <path d="M25 10H40C40 10 40 25 40 40H25V10Z" fill="black"/>
               <path d="M10 10L25 0L40 10" fill="black"/>
            </svg>
            <span class="text-3xl font-light tracking-[0.2em] uppercase text-gray-900">SolidDom</span>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">Soliddom sp. z o.o.</span>
      </div>

      <!-- Client 4: Linea -->
      <div class="bg-white p-16 flex flex-col items-center justify-center aspect-[4/3] hover:bg-gray-50 transition-colors group">
         <div class="flex flex-col items-start mb-8 grayscale group-hover:grayscale-0 transition-all duration-500">
            <div class="flex items-center gap-2">
               <div class="h-8 w-8 bg-[#E65100]"></div>
               <span class="text-4xl font-bold tracking-widest uppercase text-gray-500">Linea</span>
            </div>
            <span class="text-[10px] uppercase tracking-widest text-gray-400 self-end mt-1 w-full text-right">Siła Miastotwórcza</span>
         </div>
         <span class="text-xs font-bold uppercase tracking-wider text-gray-900">LINEA sp. z o.o.</span>
      </div>
    </div>
  </div>
</section>