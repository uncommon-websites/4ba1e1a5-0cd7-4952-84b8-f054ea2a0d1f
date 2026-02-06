<script lang="ts">
  import { onMount } from 'svelte';
</script>

<header class="w-full px-8 py-6 border-b border-white/10 flex justify-between items-center z-50 bg-dark-green text-pale-green">
    <div class="text-sm font-medium tracking-wide opacity-90">
        Autonomous Fleet Infrastructure
    </div>
    
    <div class="text-xl font-medium tracking-tight absolute left-1/2 transform -translate-x-1/2">
        <a href="/">Ark Robotics</a>
    </div>
    
    <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" class="text-sm font-medium flex items-center gap-1 opacity-90 hover:opacity-100 transition-opacity">
        LinkedIn
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <line x1="7" y1="17" x2="17" y2="7"></line>
            <polyline points="7 7 17 7 17 17"></polyline>
        </svg>
    </a>
</header>