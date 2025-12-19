<script lang="ts">
  const steps = [
    {
      id: "01",
      title: "Initial Contact and Needs Assessment",
      description: "We start with a conversation to understand your vision, requirements, and the unique characteristics of your space."
    },
    {
      id: "02",
      title: "Detailed Consultation and Site Analysis",
      description: "A thorough on-site analysis to gather data, measure the area, and assess environmental conditions."
    },
    {
      id: "03",
      title: "Concept Creation and Design Proposal",
      description: "Developing initial sketches and mood boards to visualize the potential of your future garden."
    },
    {
      id: "04",
      title: "Plant and Material Selection",
      description: "Choosing the right plants and materials that fit the design, climate, and maintenance preferences."
    },
    {
      id: "05",
      title: "Visualizations and Final Adjustments",
      description: "Creating detailed 3D visualizations to give you a realistic preview and making any necessary refinements."
    },
    {
      id: "06",
      title: "Documentation Handover",
      description: "Providing all necessary technical drawings and planting plans for the implementation team."
    }
  ];
</script>

<section class="bg-white text-gray-900 py-24 px-6 md:px-12">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="flex justify-between items-center mb-12 border-b border-gray-200 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">Simple and Clear Work Process</span>
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">(2023)</span>
    </div>

    <!-- Main Headline -->
    <h2 class="text-4xl md:text-5xl font-light leading-tight mb-24 max-w-4xl">
      Garden design is an <span class="font-serif italic">exciting journey</span> — and the process 
      from the first contact to the final project is structured to be smooth, transparent, and inspiring.
    </h2>

    <div class="grid grid-cols-1 lg:grid-cols-12 gap-16">
      <!-- Sticky Image -->
      <div class="lg:col-span-5 relative hidden lg:block">
        <div class="sticky top-12 h-[600px] w-full bg-gray-100 overflow-hidden">
           <img src="https://images.unsplash.com/photo-1584464591361-9e7530660a54?q=80&w=1000&auto=format&fit=crop" alt="Garden process" class="w-full h-full object-cover" />
        </div>
      </div>

      <!-- Steps List -->
      <div class="lg:col-span-7 space-y-0">
        {#each steps as step}
          <div class="group border-b border-gray-200 py-12 first:pt-0 flex gap-8 items-start hover:bg-gray-50/50 transition-colors px-4 -mx-4">
            <span class="text-xs font-mono text-gray-400 mt-2">({step.id})</span>
            <div class="flex-1">
              <h3 class="text-2xl font-light mb-4 group-hover:text-dark-green transition-colors">{step.title}</h3>
              <p class="text-gray-500 font-light leading-relaxed max-w-md opacity-0 h-0 overflow-hidden group-hover:opacity-100 group-hover:h-auto transition-all duration-500">
                {step.description}
              </p>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>