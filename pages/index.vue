<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section class="relative py-24 md:py-40 bg-gray-900 overflow-hidden">
      <!-- Animated background elements -->
      <div class="absolute inset-0 overflow-hidden">
        <div class="absolute top-20 left-10 w-72 h-72 bg-primary-500/20 rounded-full blur-3xl animate-pulse"></div>
        <div class="absolute bottom-20 right-10 w-96 h-96 bg-[var(--color-accent-pink)]/20 rounded-full blur-3xl animate-pulse delay-1000"></div>
        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-[600px] h-[600px] bg-[var(--color-accent-yellow)]/10 rounded-full blur-3xl"></div>
      </div>
      
      <div class="container mx-auto px-4 relative z-10">
        <div class="max-w-4xl mx-auto text-center">
          <!-- Glitch-style name -->
          <h1 class="text-5xl md:text-7xl lg:text-8xl font-display font-bold mb-6 leading-tight">
            <span class="relative inline-block">
              <span class="bg-[var(--color-accent-yellow)] px-4 py-2 transform -rotate-2 inline-block border-black border-4 shadow-neo text-black">Mehdi</span>
            </span>
            <br class="md:hidden">
            <span class="relative inline-block mt-2 md:mt-0 md:ml-4">
              <span class="bg-primary-500 text-white px-4 py-2 transform rotate-1 inline-block border-black border-4 shadow-neo">Harzallah</span>
            </span>
          </h1>
          
          <!-- Tagline with typewriter effect -->
          <div class="mb-8">
            <p class="text-xl md:text-2xl font-medium text-white/90 mb-4">
              <span class="bg-gray-800 border-2 border-white/20 px-4 py-2 inline-block transform -rotate-1">
                Software Engineer · Frontend · DevOps · Product Thinker
              </span>
            </p>
          </div>
          
          <!-- Manifesto -->
          <div class="max-w-2xl mx-auto mb-10">
            <p class="text-lg md:text-xl text-gray-300 leading-relaxed">
              I build systems, interfaces, and ideas.<br>
              Some are clean. Some are messy.<br>
              <span class="text-[var(--color-accent-pink)] font-medium">All of them try to solve real problems.</span>
            </p>
          </div>
          
          <!-- Scroll indicator -->
          <div class="flex flex-col items-center gap-4">
            <p class="text-sm text-gray-500 font-mono tracking-wider uppercase">Scroll slowly. This is not a normal portfolio.</p>
            <div class="w-px h-16 bg-gradient-to-b from-white/50 to-transparent animate-bounce"></div>
          </div>
        </div>
      </div>
      
      <!-- Decorative corners -->
      <div class="absolute bottom-0 left-0 w-32 h-32 bg-[var(--color-accent-pink)] border-black border-4 transform -translate-x-1/2 translate-y-1/2 rotate-45"></div>
      <div class="absolute top-0 right-0 w-24 h-24 bg-primary-400 border-black border-4 transform translate-x-1/2 -translate-y-1/2"></div>
    </section>
    
    <!-- Hello Section -->
    <section id="about" class="py-20 bg-gray-200 relative overflow-hidden">
      <div class="absolute -left-10 top-0 w-32 h-32 bg-primary-400 border-black border-3 transform rotate-12 z-0"></div>
      <div class="absolute right-0 bottom-0 w-24 h-24 bg-[var(--color-accent-orange)] border-black border-3 z-0"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-12 text-center relative z-10">
          <span class="bg-[var(--color-accent-yellow)] px-3 py-1 transform inline-block -rotate-2 border-black border-3 shadow-neo-sm">🧠 Hello (or whatever this is)</span>
        </h2>
        
        <div class="flex flex-col md:flex-row gap-12 items-center relative z-10">
          <div class="md:w-1/3">
            <NeoCard bgColor="white" shadow="lg" rounded="none" class="p-4 transform rotate-2">
              <div class="aspect-square bg-gray-900 dark:bg-gray-700 overflow-hidden relative border-black border-3">
                <div class="absolute inset-0 flex items-center justify-center text-gray-400 dark:text-gray-500">
                  <NuxtImg src="https://cdn.coconutstudio.io/me/me.webp" alt="Mehdi Harzallah" class="w-full h-full object-cover" />
                </div>
              </div>
              <div class="flex justify-center mt-4">
                <NeoButton variant="secondary" size="sm">
                  Systems Builder
                </NeoButton>
              </div>
            </NeoCard>
          </div>
          
          <div class="md:w-2/3">
            <NeoCard bgColor="gray" shadow="lg" class="p-6 bg-gray-900">
              <p class="text-lg mb-6 text-gray-300">
                Hi. I'm <span class="font-bold text-white">Mehdi</span>.
              </p>
              <p class="text-lg mb-6 text-gray-300">
                I'm a software engineer who:
              </p>
              <ul class="text-lg mb-6 text-gray-300 space-y-2 ml-4">
                <li class="flex items-center gap-3">
                  <span class="w-2 h-2 bg-[var(--color-accent-pink)] transform rotate-45"></span>
                  thinks in <span class="font-bold text-primary-400">systems</span>
                </li>
                <li class="flex items-center gap-3">
                  <span class="w-2 h-2 bg-[var(--color-accent-yellow)] transform rotate-45"></span>
                  sketches before coding
                </li>
                <li class="flex items-center gap-3">
                  <span class="w-2 h-2 bg-[var(--color-accent-orange)] transform rotate-45"></span>
                  <span class="font-bold text-[var(--color-accent-pink)]">breaks things</span> (intentionally)
                </li>
                <li class="flex items-center gap-3">
                  <span class="w-2 h-2 bg-primary-500 transform rotate-45"></span>
                  rebuilds them cleaner, faster, and cheaper
                </li>
              </ul>
              <p class="text-lg text-gray-300">
                I work at the intersection of <span class="bg-primary-500 text-white px-2">frontend</span>, <span class="bg-[var(--color-accent-orange)] text-white px-2">DevOps</span>, and <span class="bg-[var(--color-accent-yellow)] text-black px-2">Agentic AI</span>.
              </p>
              <p class="text-lg text-gray-300 mt-4">
                I care about performance, developer experience, and not wasting human time.
              </p>
            </NeoCard>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Experiments (Projects) Section -->
    <section id="projects" class="py-20 bg-green-400 relative overflow-hidden">
      <div class="container mx-auto px-4">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-4 text-center relative z-10">
          <span class="bg-[var(--color-accent-yellow)] px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm">
            🧪 Experiments
          </span>
        </h2>
        <p class="text-center text-black/70 mb-12 text-lg">(aka Projects)</p>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10">
          <!-- Project 1: Feeef -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-[var(--color-accent-pink)] border-black border-3 flex items-center justify-center transform rotate-12">
                <span class="font-bold text-white">🌪️</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-gradient-to-br from-primary-600 to-primary-800 border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center opacity-20">
                  <div class="w-32 h-32 bg-white border-black border-3 transform rotate-45"></div>
                </div>
                <div class="relative z-10 text-white text-center">
                  <Icon name="mdi:shopping" class="h-16 w-16 mx-auto mb-2" />
                  <span class="font-bold text-xl">Feeef</span>
                </div>
              </div>
              <h3 class="text-2xl font-bold mb-2 text-black">E-commerce SaaS</h3>
              <p class="text-sm text-gray-600 italic mb-3 border-l-4 border-[var(--color-accent-pink)] pl-3">"Not Shopify. Not trying to be."</p>
              <p class="text-gray-800 mb-4">
                Built for local sellers and real constraints. Focus on speed, simplicity, and automation.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Nuxt</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Vue</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Node.js</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Docker</span>
              </div>
              <div class="flex items-center justify-between mb-4">
                <span class="text-xs font-mono text-gray-500">Active / Iterating</span>
                <span class="text-lg">🌪️🌪️🌪️</span>
              </div>
              <NeoButton variant="primary" size="sm" class="w-full" @click="openUrl('https://feeef.net')">Visit feeef.net</NeoButton>
            </NeoCard>
          </div>
          
          <!-- Project 2: Coconut Studio -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-secondary-500 border-black border-3 flex items-center justify-center transform -rotate-12">
                <span class="font-bold text-white">🥥</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-gradient-to-br from-[var(--color-accent-yellow)] to-[var(--color-accent-orange)] border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center opacity-20">
                  <div class="w-32 h-32 bg-white border-black border-3 transform -rotate-12"></div>
                </div>
                <div class="relative z-10 text-black text-center">
                  <Icon name="mdi:palette" class="h-16 w-16 mx-auto mb-2" />
                  <span class="font-bold text-xl">Coconut Studio</span>
                </div>
              </div>
              <h3 class="text-2xl font-bold mb-2 text-black">Visual Workspace</h3>
              <p class="text-gray-800 mb-4">
                Shared space to sketch, upload, and iterate. One click from idea → prototype. Designed for speed and collaboration.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Nuxt</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Canvas APIs</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Motion</span>
              </div>
              <div class="flex items-center justify-between mb-4">
                <span class="text-xs font-mono text-gray-500">Prototype / R&D</span>
                <span class="text-lg">🌪️🌪️🌪️🌪️</span>
              </div>
              <NeoButton variant="yellow" size="sm" class="w-full" @click="openUrl('https://coconutstudio.io')">Visit coconutstudio.io</NeoButton>
            </NeoCard>
          </div>
          
          <!-- Project 3: Thirra -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-[var(--color-accent-orange)] border-black border-3 flex items-center justify-center transform rotate-12">
                <span class="font-bold text-white">🤖</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-gradient-to-br from-gray-800 to-gray-900 border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center opacity-20">
                  <div class="w-32 h-32 bg-white border-black border-3 transform rotate-12"></div>
                </div>
                <div class="relative z-10 text-white text-center">
                  <Icon name="mdi:robot" class="h-16 w-16 mx-auto mb-2" />
                  <span class="font-bold text-xl">Thirra</span>
                </div>
              </div>
              <h3 class="text-2xl font-bold mb-2 text-black">Agentic AI Infrastructure</h3>
              <p class="text-gray-800 mb-4">
                Built on top of LangChain/LangGraph. Node/workflow based AI orchestration with focus on structure and presets.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">LangChain</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">LangGraph</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">AI Agents</span>
              </div>
              <div class="flex items-center justify-between">
                <span class="text-xs font-mono text-gray-500">Experimental</span>
                <span class="text-lg">🌪️🌪️</span>
              </div>
            </NeoCard>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Experience Timeline Section -->
    <section id="experience" class="py-20 bg-sky-400 text-white relative overflow-hidden">
      <div class="container mx-auto px-4 relative z-10">
        <div class="absolute top-0 right-20 w-20 h-20 bg-[var(--color-accent-pink)] border-black border-3 transform -rotate-12"></div>
        <div class="absolute bottom-0 left-10 w-32 h-32 bg-primary-400 border-black border-3 transform rotate-6"></div>
        
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-4 text-center relative z-10">
          <span class="bg-primary-500 px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm">
            🕒 Experience
          </span>
        </h2>
        <p class="text-center text-white/70 mb-16 text-lg">(Living Timeline)</p>
        
        <div class="relative max-w-5xl mx-auto">
          <!-- Timeline Line -->
          <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2 h-full w-3 bg-black border-l-3 border-r-3 border-black"></div>
          
          <!-- Timeline Items -->
          <div class="space-y-24">
            <!-- Goubba -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-yellow)] z-20 flex items-center justify-center">
                <span class="font-bold text-black">1</span>
              </div>
              
              <div class="ml-0 md:ml-auto md:w-[calc(50%-30px)] md:pr-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1" hover>
                  <div class="absolute -top-5 -left-5 px-3 py-1 bg-[var(--color-accent-pink)] text-white border-black border-3 rotate-6">
                    07/2025 — Present
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Software Engineer</h3>
                  <div class="bg-primary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform rotate-1">
                    <span class="text-primary-800 font-medium">Goubba · Hydra, Algiers</span>
                  </div>
                  <p class="text-gray-600 text-sm mb-3">Digital gift cards & payment solutions startup</p>
                  <ul class="text-gray-800 space-y-2 text-sm">
                    <li>• Built responsive Vue.js components from AI/design mockups</li>
                    <li>• Collaborated on frontend architecture for performance</li>
                    <li>• DevOps support: CI/CD, Docker, environment config</li>
                  </ul>
                </NeoCard>
              </div>
            </div>
            
            <!-- Gosim -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-orange)] z-20 flex items-center justify-center">
                <span class="font-bold text-black">2</span>
              </div>
              
              <div class="mr-0 md:mr-auto md:w-[calc(50%-30px)] md:ml-auto md:pl-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1" hover>
                  <div class="absolute -top-5 -right-5 px-3 py-1 bg-[var(--color-accent-orange)] text-white border-black border-3 -rotate-6">
                    07/2025 — Present
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Software Engineer</h3>
                  <div class="bg-secondary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform -rotate-1">
                    <span class="text-secondary-800 font-medium">Gosim · Hydra, Algiers</span>
                  </div>
                  <ul class="text-gray-800 space-y-2 text-sm">
                    <li>• Developing and maintaining front-end applications</li>
                    <li>• Mobile app development</li>
                    <li>• Automated deployment processes</li>
                  </ul>
                </NeoCard>
              </div>
            </div>
            
            
            
            <!-- N'RICH -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-secondary-500 z-20 flex items-center justify-center">
                <span class="font-bold text-white">3</span>
              </div>
              
              <div class="mr-0 md:mr-auto md:w-[calc(50%-30px)] md:ml-auto md:pl-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1" hover>
                  <div class="absolute -top-5 -right-5 px-3 py-1 bg-secondary-500 text-white border-black border-3 -rotate-6">
                    02/2025 — 07/2025
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Angular Developer</h3>
                  <div class="bg-secondary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform -rotate-1">
                    <span class="text-secondary-800 font-medium">N'RICH · USA</span>
                  </div>
                  <ul class="text-gray-800 space-y-2 text-sm">
                    <li>• Front-end web development with Angular</li>
                    <li>• Micro front-end architecture implementation</li>
                  </ul>
                </NeoCard>
              </div>
            </div>
            
            <!-- Muthabr -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-pink)] z-20 flex items-center justify-center">
                <span class="font-bold text-white">4</span>
              </div>
              
              <div class="ml-0 md:ml-auto md:w-[calc(50%-30px)] md:pr-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1" hover>
                  <div class="absolute -top-5 -left-5 px-3 py-1 bg-[var(--color-accent-pink)] text-white border-black border-3 rotate-6">
                    2024
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Software Engineer</h3>
                  <div class="bg-primary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform rotate-1">
                    <span class="text-primary-800 font-medium">Muthabr · Oman</span>
                  </div>
                  <ul class="text-gray-800 space-y-2 text-sm">
                    <li>• Angular & Vue.js development</li>
                    <li>• Full-stack web application development</li>
                  </ul>
                </NeoCard>
              </div>
            </div>
            
            <!-- Feeef -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-yellow)] z-20 flex items-center justify-center">
                <span class="font-bold text-black">5</span>
              </div>
              
              <div class="mr-0 md:mr-auto md:w-[calc(50%-30px)] md:ml-auto md:pl-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1" hover>
                  <div class="absolute -top-5 -right-5 px-3 py-1 bg-[var(--color-accent-yellow)] text-black border-black border-3 -rotate-6">
                    2024
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Founder / Engineer</h3>
                  <div class="bg-secondary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform -rotate-1">
                    <span class="text-secondary-800 font-medium">Feeef</span>
                  </div>
                  <ul class="text-gray-800 space-y-2 text-sm">
                    <li>• Product vision, development & infrastructure</li>
                    <li>• E-commerce SaaS for Algerian market</li>
                    <li>• Business + tech + execution</li>
                  </ul>
                </NeoCard>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    
    <!-- How I Work Section -->
    <section class="py-20 bg-gray-900 text-white relative overflow-hidden">
      <div class="absolute top-0 left-0 w-24 h-24 bg-[var(--color-accent-yellow)] border-black border-3 transform -rotate-12"></div>
      <div class="absolute bottom-0 right-0 w-32 h-32 bg-primary-500 border-black border-3 transform rotate-12"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-12 text-center">
          <span class="bg-[var(--color-accent-pink)] px-3 py-1 transform inline-block -rotate-1 border-black border-3 shadow-neo-sm">
            🧩 How I Work
          </span>
        </h2>
        
        <div class="max-w-3xl mx-auto">
          <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
            <div class="bg-gray-800 p-6 border-3 border-white/20 transform -rotate-1 hover:rotate-0 transition-transform">
              <div class="w-12 h-12 bg-[var(--color-accent-yellow)] border-black border-3 flex items-center justify-center mb-4">
                <Icon name="mdi:target" class="h-6 w-6 text-black" />
              </div>
              <p class="text-lg">I start from <span class="font-bold text-[var(--color-accent-yellow)]">constraints</span></p>
            </div>
            
            <div class="bg-gray-800 p-6 border-3 border-white/20 transform rotate-1 hover:rotate-0 transition-transform">
              <div class="w-12 h-12 bg-primary-500 border-black border-3 flex items-center justify-center mb-4">
                <Icon name="mdi:sitemap" class="h-6 w-6 text-white" />
              </div>
              <p class="text-lg">I design <span class="font-bold text-primary-400">systems</span>, not just features</p>
            </div>
            
            <div class="bg-gray-800 p-6 border-3 border-white/20 transform rotate-1 hover:rotate-0 transition-transform">
              <div class="w-12 h-12 bg-[var(--color-accent-orange)] border-black border-3 flex items-center justify-center mb-4">
                <Icon name="mdi:puzzle" class="h-6 w-6 text-white" />
              </div>
              <p class="text-lg">I prefer <span class="font-bold text-[var(--color-accent-orange)]">small, composable</span> solutions</p>
            </div>
            
            <div class="bg-gray-800 p-6 border-3 border-white/20 transform -rotate-1 hover:rotate-0 transition-transform">
              <div class="w-12 h-12 bg-[var(--color-accent-pink)] border-black border-3 flex items-center justify-center mb-4">
                <Icon name="mdi:robot" class="h-6 w-6 text-white" />
              </div>
              <p class="text-lg">I <span class="font-bold text-[var(--color-accent-pink)]">automate</span> anything that repeats</p>
            </div>
            
            <div class="bg-gray-800 p-6 border-3 border-white/20 transform -rotate-1 hover:rotate-0 transition-transform md:col-span-2">
              <div class="w-12 h-12 bg-secondary-500 border-black border-3 flex items-center justify-center mb-4">
                <Icon name="mdi:lightbulb" class="h-6 w-6 text-white" />
              </div>
              <p class="text-lg">I value <span class="font-bold text-secondary-400">clarity over cleverness</span></p>
            </div>
          </div>
          
          <p class="text-center mt-8 text-xl text-gray-400">
            And yes — I care a lot about <span class="font-bold text-white bg-primary-500 px-2">DX</span>.
          </p>
        </div>
      </div>
    </section>
    
    <!-- What I'm Interested In Section -->
    <section class="py-20 bg-[var(--color-accent-yellow)] relative overflow-hidden">
      <div class="absolute bottom-0 right-0 w-24 h-24 bg-[var(--color-accent-orange)] border-black border-3 transform rotate-12"></div>
      <div class="absolute top-10 left-0 w-32 h-32 bg-primary-600 border-black border-3 transform -rotate-6"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-12 text-center">
          <span class="bg-white px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm text-black">
            🧠 What I'm Interested In (Lately)
          </span>
        </h2>
        
        <div class="max-w-4xl mx-auto">
          <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
            <NeoCard bgColor="white" shadow="md" class="p-4 transform -rotate-1 hover:rotate-0 transition-transform">
              <div class="flex items-center gap-3">
                <span class="text-2xl">🛠️</span>
                <span class="font-bold text-black">Developer platforms</span>
              </div>
            </NeoCard>
            
            <NeoCard bgColor="white" shadow="md" class="p-4 transform rotate-1 hover:rotate-0 transition-transform">
              <div class="flex items-center gap-3">
                <span class="text-2xl">🏠</span>
                <span class="font-bold text-black">Local-first / sovereign infrastructure</span>
              </div>
            </NeoCard>
            
            <NeoCard bgColor="white" shadow="md" class="p-4 transform -rotate-1 hover:rotate-0 transition-transform">
              <div class="flex items-center gap-3">
                <span class="text-2xl">🌍</span>
                <span class="font-bold text-black">SaaS for underserved markets</span>
              </div>
            </NeoCard>
            
            <NeoCard bgColor="white" shadow="md" class="p-4 transform rotate-1 hover:rotate-0 transition-transform">
              <div class="flex items-center gap-3">
                <span class="text-2xl">⚡</span>
                <span class="font-bold text-black">Tooling that reduces friction</span>
              </div>
            </NeoCard>
            
            <NeoCard bgColor="white" shadow="md" class="p-4 transform -rotate-1 hover:rotate-0 transition-transform md:col-span-2 lg:col-span-2">
              <div class="flex items-center gap-3">
                <span class="text-2xl">📈</span>
                <span class="font-bold text-black">Systems that scale without burning people out</span>
              </div>
            </NeoCard>
          </div>
        </div>
      </div>
    </section>
    
    <!-- CV Section -->
    <section class="py-16 bg-gray-200 relative overflow-hidden">
      <div class="container mx-auto px-4 relative z-10">
        <div class="max-w-2xl mx-auto text-center">
          <h2 class="text-3xl md:text-4xl font-display font-bold mb-6">
            <span class="bg-primary-500 text-white px-3 py-1 transform inline-block -rotate-1 border-black border-3">
              📄 CV (For Serious People)
            </span>
          </h2>
          
          <p class="text-lg text-gray-700 mb-6">
            If you need the structured, boring version:
          </p>
          
          <NeoButton variant="yellow" @click="downloadResume" class="transform hover:scale-105 transition-transform">
            <div class="flex items-center gap-2">
              <Icon name="mdi:download" class="h-5 w-5" />
              Download CV (PDF)
            </div>
          </NeoButton>
          
          <p class="text-sm text-gray-500 mt-6 italic">
            Otherwise, the site already tells you more than a list ever will.
          </p>
        </div>
      </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-900 text-white relative overflow-hidden">
      <div class="absolute bottom-0 right-0 w-24 h-24 bg-[var(--color-accent-pink)] border-black border-3 transform -rotate-6"></div>
      <div class="absolute top-10 left-10 w-20 h-20 bg-[var(--color-accent-yellow)] border-black border-3 transform rotate-12"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 text-center">
          <span class="bg-[var(--color-accent-orange)] px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm text-black">
            📬 Let's Build Something Weird
          </span>
        </h2>
        
        <div class="max-w-3xl mx-auto text-center mb-12">
          <p class="text-lg text-gray-300 mb-4">If you want to:</p>
          <div class="flex flex-wrap justify-center gap-3 mb-8">
            <span class="bg-gray-800 border-2 border-white/20 px-4 py-2">build a product</span>
            <span class="bg-gray-800 border-2 border-white/20 px-4 py-2">fix a system</span>
            <span class="bg-gray-800 border-2 border-white/20 px-4 py-2">ship faster</span>
            <span class="bg-gray-800 border-2 border-white/20 px-4 py-2">or just talk ideas</span>
          </div>
        </div>
        
        <div class="max-w-2xl mx-auto">
          <NeoCard bgColor="white" shadow="lg" class="p-8 transform -rotate-1">
            <div class="space-y-6">
              <a href="https://github.com/opestro" target="_blank" rel="noopener noreferrer" class="flex items-center text-black hover:text-primary-600 transition group">
                <div class="w-14 h-14 bg-gray-900 border-black border-3 flex items-center justify-center text-white mr-4 transform group-hover:rotate-6 transition-transform">
                  <Icon name="mdi:github" class="h-7 w-7" />
                </div>
                <div>
                  <span class="text-lg font-bold block">GitHub</span>
                  <span class="text-gray-600">github.com/opestro</span>
                </div>
              </a>
              
              <a href="https://linkedin.com/in/mehdi-harzallah" target="_blank" rel="noopener noreferrer" class="flex items-center text-black hover:text-primary-600 transition group">
                <div class="w-14 h-14 bg-primary-600 border-black border-3 flex items-center justify-center text-white mr-4 transform group-hover:rotate-6 transition-transform">
                  <Icon name="mdi:linkedin" class="h-7 w-7" />
                </div>
                <div>
                  <span class="text-lg font-bold block">LinkedIn</span>
                  <span class="text-gray-600">linkedin.com/in/mehdi-harzallah</span>
                </div>
              </a>
              
              <a href="mailto:mahdiharzallah21@gmail.com" class="flex items-center text-black hover:text-primary-600 transition group">
                <div class="w-14 h-14 bg-[var(--color-accent-pink)] border-black border-3 flex items-center justify-center text-white mr-4 transform group-hover:rotate-6 transition-transform">
                  <Icon name="mdi:email" class="h-7 w-7" />
                </div>
                <div>
                  <span class="text-lg font-bold block">Email</span>
                  <span class="text-gray-600">mahdiharzallah21@gmail.com</span>
                </div>
              </a>
            </div>
          </NeoCard>
        </div>
        
        <p class="text-center text-gray-500 mt-12 text-sm">
          Or don't. I'll probably still be building something.
        </p>
      </div>
    </section>
    
    <!-- Footer -->
    <footer class="py-8 bg-black text-white/50 text-center">
      <p class="text-sm italic">End of chaos. For now.</p>
    </footer>
  </div>
</template>

<script setup>
function scrollToElement(selector) {
  const element = document.querySelector(selector);
  if (element) {
    element.scrollIntoView({ behavior: 'smooth' });
  }
}

function downloadResume() {
  const link = document.createElement('a');
  link.href = 'https://cdn.coconutstudio.io/me/Mehdi-Harzallah-CV-2026.pdf';
  link.download = 'Mehdi-Harzallah-Resume.pdf';
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}

function openUrl(url) {
  window.open(url, '_blank');
}
</script>
