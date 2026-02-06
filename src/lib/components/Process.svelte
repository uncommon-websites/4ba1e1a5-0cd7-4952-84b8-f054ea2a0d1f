<script lang="ts">
  const steps = [
    {
      id: "01",
      title: "NATO Procurement & Alignment",
      description: "We reach European defense ministries through established NATO procurement channels, ensuring regulatory compliance."
    },
    {
      id: "02",
      title: "Battlefield Data Integration",
      description: "Leveraging real-world Ukrainian deployment data to overcome integration fears and prove system reliability."
    },
    {
      id: "03",
      title: "Fleet Infrastructure Setup",
      description: "Deploying the networked infrastructure required for collaborative autonomy across diverse robotic platforms."
    },
    {
      id: "04",
      title: "Mission-Level Autonomy Training",
      description: "Configuring the software for specific mission types, from frontline operations to border security."
    },
    {
      id: "05",
      title: "Collaborative Fleet Deployment",
      description: "Scaling from single units to coordinated fleets of thousands, enabling real-time battlefield dominance."
    },
    {
      id: "06",
      title: "Continuous Operational Support",
      description: "Providing ongoing technical support and software updates based on live mission feedback and evolving threats."
    }
  ];
</script>

<section id="missions" class="bg-white text-gray-900 py-24 px-6 md:px-12">
  <div class="max-w-7xl mx-auto">
    <!-- Top Label -->
    <div class="flex justify-between items-center mb-12 border-b border-gray-200 pb-4">
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">Strategic Deployment Process</span>
      <span class="text-xs uppercase tracking-widest font-medium text-gray-500">(2025)</span>
    </div>

    <!-- Main Headline -->
    <h2 class="text-4xl md:text-5xl font-light leading-tight mb-24 max-w-4xl">
      Deploying autonomous fleets is a <span class="font-serif italic">strategic mission</span> — our process 
      is designed for speed, security, and battlefield effectiveness.
    </h2>

    <div class="grid grid-cols-1 lg:grid-cols-12 gap-16">
      <!-- Sticky Image -->
      <div class="lg:col-span-5 relative hidden lg:block">
        <div class="sticky top-12 h-[600px] w-full bg-gray-100 overflow-hidden">
           <img src="https://images.unsplash.com/photo-1551808198-b30a64abb1f0?q=80&w=1000&auto=format&fit=crop" alt="Defense Deployment" class="w-full h-full object-cover" />
        </div>
      </div>

      <!-- Steps List -->
      <div class="lg:col-span-7 space-y-0">
        {#each steps as step}
          <div class="group border-b border-gray-200 py-12 first:pt-0 flex gap-8 items-start hover:bg-gray-50/50 transition-colors px-4 -mx-4">
            <span class="text-xs font-mono text-gray-400 mt-2">({step.id})</span>
            <div class="flex-1">
              <h3 class="text-2xl font-light mb-4 group-hover:text-primary-500 transition-colors">{step.title}</h3>
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