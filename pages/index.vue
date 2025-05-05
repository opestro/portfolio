<template>
  <div>
    <!-- Hero Section -->
    <section class="relative py-20 md:py-32 bg-gray-200 overflow-hidden">
      <div class="container mx-auto px-4 relative z-10">
        <div class="max-w-4xl mx-auto">
          <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
            <!-- Text Content -->
            <div class="flex flex-col justify-center">
              <h1 class="text-5xl md:text-6xl lg:text-7xl font-display font-bold mb-6 leading-tight">
                <span class="bg-[var(--color-accent-yellow)] px-2 transform -rotate-1 inline-block">Mehdi</span> 
                <span class="bg-primary-500 text-white px-2 transform rotate-1 inline-block">Harzallah</span>
              </h1>
              <p class="text-xl md:text-2xl font-medium mb-8 transform -rotate-1 bg-gray-700 border-black border-3 p-4 shadow-neo-sm inline-block text-white">
                Developer & Civil Engineer Innovator
              </p>
              <p class="text-lg mb-8 bg-gray-700 p-4 border-black border-3 text-white">
                Where <span class="font-bold text-[var(--color-accent-pink)]">Smart Code</span> Meets 
                <span class="font-bold text-primary-600">Solid Structures</span>.
                I build scalable software, smart tools, and bridge the gap between code and concrete.
              </p>
              <div class="flex flex-wrap gap-4">
                <NeoButton variant="primary" @click="scrollToElement('#projects')">
                  View My Work
                </NeoButton>
                <NeoButton variant="yellow" @click="downloadResume">
                  Download Resume
                </NeoButton>
              </div>
            </div>
            
            <!-- Hero Pattern/Image -->
            <div class="relative hidden lg:block">
              <div class="absolute -right-20 top-0 w-96 h-96 bg-[var(--color-accent-yellow)] border-black border-3 rounded-full transform rotate-12 z-0"></div>
              <div class="absolute right-20 top-20 w-64 h-64 bg-primary-400 border-black border-3 transform -rotate-6 z-10"></div>
              <div class="absolute right-10 top-32 w-80 h-80 bg-secondary-400 border-black border-3 transform rotate-3 z-20"></div>
              <div class="absolute right-40 top-40 w-60 h-60 bg-white border-black border-3 flex items-center justify-center z-30">
                <div class="text-6xl font-bold transform -rotate-6">
                  <span class="text-primary-500">M</span><span class="text-[var(--color-accent-pink)]">H</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      
      <!-- Decorative Elements -->
      <div class="absolute bottom-0 left-0 w-24 h-24 bg-[var(--color-accent-pink)] border-black border-3"></div>
      <div class="absolute top-0 right-0 w-48 h-48 bg-secondary-300 border-black border-3 transform rotate-45 -translate-y-1/2 translate-x-1/4"></div>
    </section>
    
    <!-- About Section -->
    <section id="about" class="py-20 bg-gray-200 ">
      <div class="container mx-auto px-4 relative">
        <div class="absolute -left-10 top-0 w-32 h-32 bg-primary-400 border-black border-3 transform rotate-12 z-0"></div>
        <div class="absolute right-0 bottom-0 w-24 h-24 bg-[var(--color-accent-orange)] border-black border-3 z-0"></div>
        
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-12 text-center relative z-10">
          <span class="bg-[var(--color-accent-yellow)] px-3 py-1 transform inline-block -rotate-2 border-black border-3 shadow-neo-sm">About Me</span>
        </h2>
        
        <div class="flex flex-col md:flex-row gap-12 items-center relative z-10">
          <div class="md:w-1/3">
            <NeoCard bgColor="white" shadow="lg" rounded="none" class="p-4 transform rotate-2">
              <div class="aspect-square bg-gray-900 dark:bg-gray-700 overflow-hidden relative border-black border-3">
                <!-- Placeholder for profile image -->
                <div class="absolute inset-0 flex items-center justify-center text-gray-400 dark:text-gray-500">
                  <NuxtImg src="/me.webp" alt="Mehdi Harzallah" class="w-full h-full object-cover" />
                </div>
              </div>
              <div class="flex justify-center mt-4">
                <NeoButton variant="secondary" size="sm">
                  Civil Engineer & Developer
                </NeoButton>
              </div>
            </NeoCard>
          </div>
          
          <div class="md:w-2/3">
            <NeoCard bgColor="gray"  shadow="lg" class="p-6 bg-gray-900">
              <p class="text-lg mb-6 text-gray-800 dark:text-gray-300">
                I'm a polymath who bridges the worlds of <span class="font-bold text-primary-600">Civil Engineering</span> and <span class="font-bold text-[var(--color-accent-pink)]">Software Development</span>, bringing a unique perspective to both fields. With a strong academic background in Civil Engineering and hands-on experience in software development, I create solutions that transform how we approach construction, design, and infrastructure management.
              </p>
              <p class="text-lg mb-6 text-gray-800 dark:text-gray-300">
                My journey began with 3D design in civil engineering, which sparked my passion for creating digital tools. Today, I specialize in <span class="bg-primary-500 text-white px-1">DevOps practices</span>, <span class="bg-[var(--color-accent-orange)] text-white px-1">full-stack web development</span>, and applying <span class="bg-[var(--color-accent-yellow)] text-black px-1">AI</span> to solve complex engineering challenges.
              </p>
              <p class="text-lg text-gray-800 dark:text-gray-300">
                I'm constantly exploring the intersection of traditional engineering principles and cutting-edge software solutions, developing tools that optimize construction processes, predict material behavior, and improve infrastructure management.
              </p>
            </NeoCard>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Experience Timeline Section -->
    <section id="experience" class="py-20 bg-sky-400 text-white">
      <div class="container mx-auto px-4 relative">
        <div class="absolute top-0 right-20 w-20 h-20 bg-[var(--color-accent-pink)] border-black border-3 transform -rotate-12"></div>
        <div class="absolute bottom-0 left-10 w-32 h-32 bg-primary-400 border-black border-3 transform rotate-6"></div>
        
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-16 text-center relative z-10">
          <span class="bg-primary-500 px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm">
            Experience
          </span>
        </h2>
        
        <div class="relative max-w-5xl mx-auto">
          <!-- Timeline Line -->
          <div class="hidden md:block absolute left-1/2 transform -translate-x-1/2 h-full w-3 bg-black border-l-3 border-r-3 border-black"></div>
          
          <!-- Timeline Items -->
          <div class="space-y-24">
            <!-- Muthabr -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-yellow)] z-20 flex items-center justify-center">
                <span class="font-bold text-black">1</span>
              </div>
              
              <div class="ml-0 md:ml-auto md:w-[calc(50%-30px)] md:pr-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1" hover>
                  <div class="absolute -top-5 -left-5 px-3 py-1 bg-[var(--color-accent-pink)] text-white border-black border-3 rotate-6">
                    Present
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Software Engineer</h3>
                  <div class="bg-primary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform rotate-1">
                    <span class="text-primary-800 font-medium">Muthabr</span>
                  </div>
                  <p class="text-gray-800">
                    Led development of scalable web applications with modern frameworks, implemented CI/CD pipelines, and integrated AI-powered features.
                  </p>
                </NeoCard>
              </div>
            </div>
            
            <!-- Feeef -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-orange)] z-20 flex items-center justify-center">
                <span class="font-bold text-black">2</span>
              </div>
              
              <div class="mr-0 md:mr-auto md:w-[calc(50%-30px)] md:ml-auto md:pl-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1" hover>
                  <h3 class="text-2xl font-bold mb-2 text-black">DevOps / Developer</h3>
                  <div class="bg-secondary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform -rotate-1">
                    <span class="text-secondary-800 font-medium">Feeef</span>
                  </div>
                  <p class="text-gray-800">
                    Managed cloud infrastructure and deployments, optimized application performance, and implemented monitoring solutions.
                  </p>
                </NeoCard>
              </div>
            </div>
            
            <!-- D&D Consulting -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-primary-500 z-20 flex items-center justify-center">
                <span class="font-bold text-white">3</span>
              </div>
              
              <div class="ml-0 md:ml-auto md:w-[calc(50%-30px)] md:pr-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1" hover>
                  <h3 class="text-2xl font-bold mb-2 text-black">DevOps Engineer</h3>
                  <div class="bg-primary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform rotate-1">
                    <span class="text-primary-800 font-medium">D&D Consulting</span>
                  </div>
                  <p class="text-gray-800">
                    Architected and maintained containerized environments, streamlined deployment processes, and automated infrastructure management.
                  </p>
                </NeoCard>
              </div>
            </div>
            
            <!-- Chronorex Express -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-secondary-500 z-20 flex items-center justify-center">
                <span class="font-bold text-white">4</span>
              </div>
              
              <div class="mr-0 md:mr-auto md:w-[calc(50%-30px)] md:ml-auto md:pl-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1" hover>
                  <h3 class="text-2xl font-bold mb-2 text-black">CMS Developer</h3>
                  <div class="bg-secondary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform -rotate-1">
                    <span class="text-secondary-800 font-medium">Chronorex Express</span>
                  </div>
                  <p class="text-gray-800">
                    Developed and customized content management solutions, integrated e-commerce functionality, and improved user experience.
                  </p>
                </NeoCard>
              </div>
            </div>
            
            <!-- Swellty -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-[var(--color-accent-pink)] z-20 flex items-center justify-center">
                <span class="font-bold text-white">5</span>
              </div>
              
              <div class="ml-0 md:ml-auto md:w-[calc(50%-30px)] md:pr-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1" hover>
                  <h3 class="text-2xl font-bold mb-2 text-black">Business Owner</h3>
                  <div class="bg-primary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform rotate-1">
                    <span class="text-primary-800 font-medium">Swellty</span>
                  </div>
                  <p class="text-gray-800">
                    Founded and managed a technology startup, developed innovative solutions, and built client relationships.
                  </p>
                </NeoCard>
              </div>
            </div>
            
            <!-- Freelance -->
            <div class="relative">
              <div class="md:absolute left-1/2 transform -translate-x-1/2 -mt-5 w-10 h-10 rounded-full border-3 border-black bg-white z-20 flex items-center justify-center">
                <span class="font-bold text-black">6</span>
              </div>
              
              <div class="mr-0 md:mr-auto md:w-[calc(50%-30px)] md:ml-auto md:pl-12 relative z-10">
                <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1" hover>
                  <div class="absolute -top-5 -right-5 px-3 py-1 bg-[var(--color-accent-yellow)] text-black border-black border-3 -rotate-6">
                    2020
                  </div>
                  <h3 class="text-2xl font-bold mb-2 text-black">Freelance Developer</h3>
                  <div class="bg-secondary-100 inline-block px-3 py-1 mb-4 border-black border-2 transform -rotate-1">
                    <span class="text-secondary-800 font-medium">CSCC, Gama Outillage, Raya</span>
                  </div>
                  <p class="text-gray-800">
                    Delivered custom web solutions, e-commerce platforms, and data-driven applications for multiple clients.
                  </p>
                </NeoCard>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Projects Section -->
    <section id="projects" class="py-20 bg-green-400 ">
      <div class="container mx-auto px-4">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-16 text-center relative z-10">
          <span class="bg-[var(--color-accent-yellow)] px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm">
            Projects
          </span>
        </h2>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10">
          <!-- Project 1: Cutting Optimizer Pro -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-[var(--color-accent-pink)] border-black border-3 flex items-center justify-center transform rotate-12">
                <span class="font-bold text-white">1</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-primary-500 border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center">
                  <div class="w-32 h-32 bg-white border-black border-3 transform rotate-45"></div>
                </div>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 text-black relative z-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 10l-2 1m0 0l-2-1m2 1v2.5M20 7l-2 1m2-1l-2-1m2 1v2.5M14 4l-2-1-2 1M4 7l2-1M4 7l2 1M4 7v2.5M12 21l-2-1m2 1l2-1m-2 1v-2.5M6 18l-2-1v-2.5M18 18l2-1v-2.5" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">Cutting Optimizer Pro</h3>
              <p class="text-gray-800 mb-4">
                AI-powered tool for metal construction optimization that minimizes waste and maximizes efficiency.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Python</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">TensorFlow</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Optimization</span>
              </div>
              <NeoButton  variant="primary" size="sm" class="w-full" @click="openUrl('https://github.com/opestro/Cutting-Optimization-Pro')">View Project</NeoButton>
            </NeoCard>
          </div>
          
          <!-- Project 2: Concrete Strength Predictor -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-secondary-500 border-black border-3 flex items-center justify-center transform -rotate-12">
                <span class="font-bold text-white">2</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-[var(--color-accent-yellow)] border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center">
                  <div class="w-32 h-32 bg-white border-black border-3 transform -rotate-12"></div>
                </div>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 text-black relative z-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">Concrete Strength Predictor</h3>
              <p class="text-gray-800 mb-4">
                ML model for structural forecasting that predicts concrete strength based on composition and curing conditions.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Python</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Scikit-learn</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Material Science</span>
              </div>
              <NeoButton variant="yellow" size="sm" class="w-full">Soon</NeoButton>
            </NeoCard>
          </div>
          
          <!-- Project 3: Docker Container Visualizer -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-[var(--color-accent-orange)] border-black border-3 flex items-center justify-center transform rotate-12">
                <span class="font-bold text-white">3</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-primary-700 border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center">
                  <div class="w-32 h-32 bg-white border-black border-3 transform rotate-12"></div>
                </div>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 text-black relative z-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">Docker Container Visualizer</h3>
              <p class="text-gray-800 mb-4">
                Real-time Docker infrastructure UI that provides visual monitoring and management of containers.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Vue.js</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Docker API</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">WebSocket</span>
              </div>
              <NeoButton variant="orange" size="sm" class="w-full" @click="openUrl('https://github.com/opestro/Docker-Container-Visualizer')">View Project</NeoButton>
            </NeoCard>
          </div>
          
          <!-- Project 4: CSDeploy -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-primary-500 border-black border-3 flex items-center justify-center transform -rotate-12">
                <span class="font-bold text-white">4</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-secondary-600 border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center">
                  <div class="w-32 h-32 bg-white border-black border-3 transform -rotate-12"></div>
                </div>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 text-black relative z-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 9l3 3-3 3m5 0h3M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">CSDeploy</h3>
              <p class="text-gray-800 mb-4">
                CLI deployment tool for developers that simplifies deployment workflows across multiple environments.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Go</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">CLI</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">DevOps</span>
              </div>
              <NeoButton variant="secondary" size="sm" class="w-full" @click="openUrl('https://github.com/opestro/csdeploy')">View Project</NeoButton>
            </NeoCard>
          </div>
          
          <!-- Project 5:  TypeORM-Visual -->
          <div class="group md:col-span-2 lg:col-span-1">
            <NeoCard bgColor="white" shadow="lg" class="p-6 relative group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="absolute z-10 -top-5 -right-5 w-12 h-12 rounded-full bg-[var(--color-accent-yellow)] border-black border-3 flex items-center justify-center transform rotate-12">
                <span class="font-bold text-black">5</span>
              </div>
              <div class="h-48 -mx-6 -mt-6 mb-6 bg-[var(--color-accent-pink)] border-b-3 border-black flex items-center justify-center p-6 overflow-hidden relative">
                <div class="absolute inset-0 flex items-center justify-center">
                  <div class="w-32 h-32 bg-white border-black border-3 transform rotate-12">
                    <!-- <NuxtImg src="/typorm.png" class=" w-full " ></NuxtImg> -->
                  </div>
                </div>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-20 w-20 text-black relative z-10" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black"> TypeORM-Visual</h3>
              <p class="text-gray-800 mb-4">
                Interactive CLI for generating TypeORM entities for NestJS applications with a nice UX.
              </p>
              <div class="flex flex-wrap gap-2 mb-4">
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">IoT</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">React</span>
                <span class="px-3 py-1 border-2 border-black bg-primary-100 text-primary-800 text-xs font-bold">Node.js</span>
              </div>
              <NeoButton variant="pink" size="sm" class="w-full" @click="openUrl('https://github.com/opestro/TypeORM-Visual')">View Project</NeoButton>
            </NeoCard>
          </div>
        </div>
      </div>
    </section>
    
    <!-- GitHub Integration Section -->
    <section id="github" class="py-20 bg-[var(--color-accent-orange)] text-white relative overflow-hidden">
      <div class="absolute top-0 left-0 w-24 h-24 bg-[var(--color-accent-yellow)] border-black border-3 transform -rotate-12"></div>
      <div class="absolute bottom-0 right-0 w-32 h-32 bg-primary-500 border-black border-3 transform rotate-12"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-6 text-center">
          <span class="bg-gray-200 text-[var(--color-accent-orange)] px-3 py-1 transform inline-block -rotate-1 border-black border-3 shadow-neo-sm">
            Open Source
          </span>
        </h2>
        <p class="text-center mb-12 max-w-2xl mx-auto">
          Check out my latest projects and contributions on GitHub. I'm passionate about open source and regularly contribute to projects that push the boundaries of technology.
        </p>
        
        <div class="flex justify-center mb-12">
          <NeoButton variant="white" @click="openUrl('https://github.com/opestro')">
            <div class="flex items-center">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2" fill="currentColor" viewBox="0 0 24 24">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.237 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
              </svg>
              Visit My GitHub Profile
            </div>
          </NeoButton>
        </div>
        
        <!-- GitHub Repositories Preview -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 max-w-5xl mx-auto">
          <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-2">
            <div class="flex items-start justify-between mb-4">
              <div>
                <h3 class="font-bold text-xl text-black mb-1">TypeORM-Visual</h3>
                <p class="text-sm text-gray-600">TypeORM Visual</p>
              </div>
              <div class="flex items-center">
                <span class="flex items-center text-[var(--color-accent-yellow)] mr-3 border-2 border-black px-2 py-1 bg-gray-900">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 .587l3.668 7.568 8.332 1.151-6.064 5.828 1.48 8.279-7.416-3.967-7.417 3.967 1.481-8.279-6.064-5.828 8.332-1.151z"/>
                  </svg>
                 13
                </span>
                <span class="flex items-center text-white border-2 border-black px-2 py-1 bg-gray-900">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M5.559 8.855c.166 1.183.789 3.207 3.087 4.079-2.863.099-6.144-.829-8.646-2.934 1.272 7.299 9.109 11 18 6l-2-1c1-.5 2.5-.5 3.5 0 .667-1 1-2 1-3 2.016-.169 3.3-1.756 4-3-1 .5-2 0-2.5-1 .279-1.346 1.305-2.332 2-3-1.5-.667-3-.5-4.5.5-1.603-2.096-3.866-2.744-6-2.5l-1 2c-1.121-1.341-2.023-2.879-2-5.5-1.5 1.5-2.5 3.5-2.5 5.5-1.603-.483-2.679-1.463-3.5-3 0 3-1.889 5.258-5 6.5z"/>
                  </svg>
                  0
                </span>
              </div>
            </div>
            <p class="text-gray-800 text-sm mb-4 border-l-4 border-primary-500 pl-3">
               Interactive CLI for generating TypeORM entities for NestJS applications with a nice UX.
            </p>
            <div class="flex items-center justify-between">
              <span class="flex items-center text-gray-600">
                <span class="w-3 h-3 rounded-full bg-yellow-500 mr-1 border border-black"></span>
                NodeJs
              </span>
              <NeoButton variant="pink" size="sm" @click="openUrl('https://github.com/opestro/TypeORM-Visual')">Fork it!</NeoButton>
            </div>
          </NeoCard>
          
          <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1">
            <div class="flex items-start justify-between mb-4">
              <div>
                <h3 class="font-bold text-xl text-black mb-1">docker-visualizer</h3>
                <p class="text-sm text-gray-600">Real-time Docker container visualization</p>
              </div>
              <div class="flex items-center">
                <span class="flex items-center text-[var(--color-accent-yellow)] mr-3 border-2 border-black px-2 py-1 bg-gray-900">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 .587l3.668 7.568 8.332 1.151-6.064 5.828 1.48 8.279-7.416-3.967-7.417 3.967 1.481-8.279-6.064-5.828 8.332-1.151z"/>
                  </svg>
                  6
                </span>
                <span class="flex items-center text-white border-2 border-black px-2 py-1 bg-gray-900">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M5.559 8.855c.166 1.183.789 3.207 3.087 4.079-2.863.099-6.144-.829-8.646-2.934 1.272 7.299 9.109 11 18 6l-2-1c1-.5 2.5-.5 3.5 0 .667-1 1-2 1-3 2.016-.169 3.3-1.756 4-3-1 .5-2 0-2.5-1 .279-1.346 1.305-2.332 2-3-1.5-.667-3-.5-4.5.5-1.603-2.096-3.866-2.744-6-2.5l-1 2c-1.121-1.341-2.023-2.879-2-5.5-1.5 1.5-2.5 3.5-2.5 5.5-1.603-.483-2.679-1.463-3.5-3 0 3-1.889 5.258-5 6.5z"/>
                  </svg>
                  0
                </span>
              </div>
            </div>
            <p class="text-gray-800 text-sm mb-4 border-l-4 border-secondary-500 pl-3">
                Beautiful Blueprint-Style Docker Container Visualization.
            </p>
            <div class="flex items-center justify-between">
              <span class="flex items-center text-gray-600">
                <span class="w-3 h-3 rounded-full bg-blue-500 mr-1 border border-black"></span>
                JavaScript
              </span>
              <NeoButton variant="secondary" size="sm" @click="openUrl('https://github.com/opestro/Docker-Container-Visualizer')">Fork it!</NeoButton>
            </div>
          </NeoCard>
        </div>
      </div>
    </section>
    
    <!-- Hackathons & Awards Section -->
    <section class="py-20 bg-[var(--color-accent-yellow)] relative overflow-hidden">
      <div class="absolute bottom-0 right-0 w-24 h-24 bg-[var(--color-accent-orange)] border-black border-3 transform rotate-12"></div>
      <div class="absolute top-10 left-0 w-32 h-32 bg-primary-600 border-black border-3 transform -rotate-6"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-16 text-center relative z-10">
          <span class="bg-[var(--color-accent-yellow)] px-3 py-1 transform inline-block rotate-2 border-black border-3 shadow-neo-sm">
            Hackathons & Awards
          </span>
        </h2>
        
        <div class="max-w-4xl mx-auto">
          <NeoCard bgColor="white" shadow="lg" class="p-8 md:p-12 transform -rotate-1">
            <div class="flex flex-col md:flex-row items-center gap-8">
              <div class="md:w-1/3 flex justify-center">
                <div class="relative">
                  <div class="w-32 h-32 bg-[var(--color-accent-pink)] border-black border-3 transform rotate-6 flex items-center justify-center">
                    <div class="w-20 h-20 bg-white border-black border-3 flex items-center justify-center">
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z" />
                      </svg>
                    </div>
                  </div>
                  <div class="absolute -top-5 -right-5 bg-[var(--color-accent-yellow)] border-black border-3 w-12 h-12 flex items-center justify-center text-black font-bold text-xl transform rotate-12">
                    1<sup>st</sup>
                  </div>
                </div>
              </div>
              <div class="md:w-2/3">
                <div class="bg-primary-100 inline-block px-3 py-1 mb-2 border-black border-2 transform -rotate-1">
                  <span class="text-primary-800 font-medium">Nest Hackathon 2025</span>
                </div>
                <h3 class="text-2xl font-bold mb-3 text-black">Smart Warehouse Robotics System</h3>
                <p class="text-gray-800 mb-4">
                  Led a team of developers and engineers to create an innovative warehouse automation system that uses IoT sensors, robotic controls, and a real-time web dashboard to optimize warehouse operations.
                </p>
                <div class="flex flex-wrap gap-3 mb-4">
                  <span class="px-3 py-1 bg-white border-black border-2 text-black text-sm transform rotate-1 inline-block">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1 inline" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                    </svg>
                    Web & IoT Developer
                  </span>
                  <span class="px-3 py-1 bg-white border-black border-2 text-black text-sm transform -rotate-1 inline-block">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1 inline" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4" />
                    </svg>
                    Sponsored by Sonatrach
                  </span>
                  <span class="px-3 py-1 bg-white border-black border-2 text-black text-sm transform rotate-1 inline-block">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 mr-1 inline" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
                    </svg>
                    Mobilis
                  </span>
                </div>
                <NeoButton variant="primary" size="sm" @click="openUrl('https://www.linkedin.com/posts/mehdi-harzallah_nesthackathon2025-astclub-cscclub-activity-7317596449855188992-OsB4?utm_source=share&utm_medium=member_desktop&rcm=ACoAADh_YhoBKU8UPAjEVxAPn5V1jOnHOPKkKeA')">Read more!</NeoButton>
              </div>
            </div>
          </NeoCard>
        </div>
      </div>
    </section>
    
    <!-- Civil Engineering Innovation Section -->
    <section class="py-20 bg-gray-200 relative overflow-hidden">
      <!-- <div class="absolute top-0 right-0 w-36 h-36 bg-primary-500 border-black border-3 transform rotate-12"></div> -->
      <div class="absolute bottom-0 left-0 w-24 h-24 bg-[var(--color-accent-yellow)] border-black border-3 transform -rotate-6"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-12 text-center relative z-10">
          <span class="bg-primary-500 text-white px-3 py-1 transform inline-block -rotate-1 border-black border-3 shadow-neo-sm">
            Civil Engineering Innovation
          </span>
        </h2>
        
        <p class="text-center text-black mb-12 max-w-3xl mx-auto bg-white border-black border-3 p-4 transform rotate-1 shadow-neo-sm">
          Bridging the gap between structural engineering principles and cutting-edge software solutions to revolutionize the construction industry.
        </p>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
          <!-- Card 1 -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1 group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="bg-[var(--color-accent-pink)] w-16 h-16 border-black border-3 flex items-center justify-center mb-6 transform rotate-3">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">AI Concrete Modeling</h3>
              <p class="text-gray-800 mb-4">
                Developed machine learning models that predict concrete strength based on mix composition and environmental factors, reducing testing time by 60%.
              </p>
              <div class="bg-primary-100 inline-block px-3 py-1 border-black border-2 transform rotate-1">
                <span class="text-primary-800 font-medium">Machine Learning</span>
              </div>
            </NeoCard>
          </div>
          
          <!-- Card 2 -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 transform rotate-1 group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="bg-[var(--color-accent-yellow)] w-16 h-16 border-black border-3 flex items-center justify-center mb-6 transform -rotate-3">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">Real-World Applications</h3>
              <p class="text-gray-800 mb-4">
                Applied AI-powered construction tools to real projects, resulting in 15% cost reduction and 30% faster project completion times.
              </p>
              <div class="bg-secondary-100 inline-block px-3 py-1 border-black border-2 transform -rotate-1">
                <span class="text-secondary-800 font-medium">Process Optimization</span>
              </div>
            </NeoCard>
          </div>
          
          <!-- Card 3 -->
          <div class="group">
            <NeoCard bgColor="white" shadow="lg" class="p-6 transform -rotate-1 group-hover:-translate-y-2 group-hover:translate-x-2 transition-all duration-300">
              <div class="bg-[var(--color-accent-orange)] w-16 h-16 border-black border-3 flex items-center justify-center mb-6 transform rotate-3">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z" />
                </svg>
              </div>
              <h3 class="text-2xl font-bold mb-3 text-black">Material Optimization</h3>
              <p class="text-gray-800 mb-4">
                Created tools that optimize material use in construction, reducing waste by 25% while maintaining structural integrity and safety standards.
              </p>
              <div class="bg-primary-100 inline-block px-3 py-1 border-black border-2 transform rotate-1">
                <span class="text-primary-800 font-medium">Sustainability</span>
              </div>
            </NeoCard>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-200 relative overflow-hidden">
      <!-- Decorative elements -->
      <!-- <div class="absolute -top-10 -left-10 w-40 h-40 bg-primary-500 z-50 border-black border-3 transform rotate-12"></div> -->
      <div class="absolute bottom-0 right-0 w-24 h-24 bg-[var(--color-accent-pink)] border-black border-3 transform -rotate-6"></div>
      
      <div class="container mx-auto px-4 relative z-10">
        <h2 class="text-4xl md:text-5xl font-display font-bold mb-12 text-center relative z-10">
          <span class="bg-[var(--color-accent-orange)] px-3 py-1 transform inline-block rotate-1 border-black border-3 shadow-neo-sm text-black">
            Get In Touch
          </span>
        </h2>
        
        <div class="max-w-5xl mx-auto">
          <NeoCard bgColor="white" shadow="lg" class="p-8 transform -rotate-1">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
              <!-- Contact Info -->
              <div>
                <h3 class="text-2xl font-bold mb-6 text-black border-b-3 border-black pb-2">Let's Connect</h3>
                <p class="text-lg mb-8 text-gray-800 bg-[var(--color-accent-yellow)] p-3 border-black border-3 transform rotate-1 inline-block">
                  Interested in collaborating on a project? I'd love to hear from you!
                </p>
                
                <div class="space-y-5">
                  <a href="mailto:mahdiharzallah21@gmail.com" class="flex items-center text-black hover:text-primary-600 transition group">
                    <div class="w-12 h-12 bg-primary-500 border-black border-3 flex items-center justify-center text-white mr-4 transform group-hover:rotate-6 transition-transform">
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                      </svg>
                    </div>
                    <span class="text-lg font-medium">mahdiharzallah21@gmail.com</span>
                  </a>
                  
                  <a href="https://linkedin.com/in/mehdi-harzallah" target="_blank" rel="noopener noreferrer" class="flex items-center text-black hover:text-primary-600 transition group">
                    <div class="w-12 h-12 bg-[var(--color-accent-pink)] border-black border-3 flex items-center justify-center text-white mr-4 transform group-hover:rotate-6 transition-transform">
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z"/>
                      </svg>
                    </div>
                    <span class="text-lg font-medium">linkedin.com/in/mehdi-harzallah</span>
                  </a>
                  
                  <a href="tel:+213778191078" class="flex items-center text-black hover:text-primary-600 transition group">
                    <div class="w-12 h-12 bg-[var(--color-accent-yellow)] border-black border-3 flex items-center justify-center text-black mr-4 transform group-hover:rotate-6 transition-transform">
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                      </svg>
                    </div>
                    <span class="text-lg font-medium">+213 778191078</span>
                  </a>
                  
                  <a href="https://github.com/opestro" target="_blank" rel="noopener noreferrer" class="flex items-center text-black hover:text-primary-600 transition group">
                    <div class="w-12 h-12 bg-primary-700 border-black border-3 flex items-center justify-center text-white mr-4 transform group-hover:rotate-6 transition-transform">
                      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.237 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                      </svg>
                    </div>
                    <span class="text-lg font-medium">github.com/opestro</span>
                  </a>
                </div>
              </div>
              
              <!-- Contact Form -->
              <div class="relative">
                <div class="absolute -top-4 -right-4 w-16 h-16 bg-[var(--color-accent-orange)] border-black border-3 transform rotate-12"></div>
                
                <div class="bg-gray-100 p-6 border-black border-3 relative">
                  <h3 class="text-2xl font-bold mb-6 text-black transform -rotate-1 inline-block">
                    Send a Message
                  </h3>
                  
                  <form>
                    <div class="mb-4">
                      <label for="name" class="block text-sm font-bold text-black mb-2 transform -rotate-1 inline-block bg-[var(--color-accent-yellow)] px-2 border-black border-2">Name</label>
                      <input type="text" id="name" name="name" class="w-full px-4 py-3 border-black border-3 focus:ring-2 focus:ring-primary-500 focus:border-primary-500 bg-white text-black">
                    </div>
                    
                    <div class="mb-4">
                      <label for="email" class="block text-sm font-bold text-black mb-2 transform rotate-1 inline-block bg-primary-100 px-2 border-black border-2">Email</label>
                      <input type="email" id="email" name="email" class="w-full px-4 py-3 border-black border-3 focus:ring-2 focus:ring-primary-500 focus:border-primary-500 bg-white text-black">
                    </div>
                    
                    <div class="mb-4">
                      <label for="subject" class="block text-sm font-bold text-black mb-2 transform -rotate-1 inline-block bg-[var(--color-accent-pink)] px-2 text-white border-black border-2">Subject</label>
                      <input type="text" id="subject" name="subject" class="w-full px-4 py-3 border-black border-3 focus:ring-2 focus:ring-primary-500 focus:border-primary-500 bg-white text-black">
                    </div>
                    
                    <div class="mb-6">
                      <label for="message" class="block text-sm font-bold text-black mb-2 transform rotate-1 inline-block bg-primary-400 px-2 text-white border-black border-2">Message</label>
                      <textarea id="message" name="message" rows="4" class="w-full px-4 py-3 border-black border-3 focus:ring-2 focus:ring-primary-500 focus:border-primary-500 bg-white text-black"></textarea>
                    </div>
                    
                    <NeoButton variant="yellow" class="w-full transform hover:-translate-y-1">
                      Send Message
                    </NeoButton>
                  </form>
                </div>
              </div>
            </div>
          </NeoCard>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

function scrollToElement(selector) {
  const element = document.querySelector(selector);
  if (element) {
    element.scrollIntoView({ behavior: 'smooth' });
  }
}

function downloadResume() {
  const link = document.createElement('a');
  link.href = '/MEHDI-RESUME.pdf';
  link.download = 'Mehdi-Harzallah-Resume.pdf';
  document.body.appendChild(link);
  link.click();
  document.body.removeChild(link);
}

function openUrl(url) {
  window.open(url, '_blank');
}
</script>

