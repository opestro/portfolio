<template>
  <div class="min-h-screen flex flex-col bg-gray-900">
    <header class="sticky top-0 z-50 bg-gray-900 border-b-3 border-black">
      <div class="container mx-auto px-4 py-4 flex justify-between items-center">
        <div class="text-xl font-bold text-white bg-primary-500 px-3 py-1 border-black border-3 transform -rotate-1 shadow-neo-sm">
          Mehdi Harzallah
        </div>
        <nav class="hidden md:flex space-x-6">
          <a href="#about" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 hover:translate-y-0.5">About</a>
          <a href="#experience" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 hover:translate-y-0.5">Experience</a>
          <a href="#projects" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 hover:translate-y-0.5">Projects</a>
          <a href="#github" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 hover:translate-y-0.5">GitHub</a>
          <a href="#contact" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 hover:translate-y-0.5">Contact</a>
        </nav>
        <div class="flex items-center space-x-3">
          <button class="p-2 bg-[var(--color-accent-yellow)] border-black border-3 text-black hover:translate-y-0.5 hover:translate-x-0.5 active:translate-y-1 active:translate-x-1 active:shadow-none shadow-neo-sm transition" 
                  @click="toggleDarkMode" aria-label="Toggle dark mode">
            <svg v-if="darkMode" xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z" />
            </svg>
            <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z" />
            </svg>
          </button>
          <button class="block md:hidden p-2 bg-[var(--color-accent-pink)] border-black border-3 text-white hover:translate-y-0.5 hover:translate-x-0.5 active:translate-y-1 active:translate-x-1 active:shadow-none shadow-neo-sm transition" 
                  @click="toggleMobileMenu" aria-label="Toggle menu">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu -->
      <div v-if="mobileMenuOpen" class="md:hidden absolute w-full bg-gray-900 border-b-3 border-black">
        <div class="container mx-auto px-4 py-3 flex flex-col space-y-3">
          <a href="#about" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 py-2 border-b border-gray-700" @click="closeMobileMenu">About</a>
          <a href="#experience" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 py-2 border-b border-gray-700" @click="closeMobileMenu">Experience</a>
          <a href="#projects" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 py-2 border-b border-gray-700" @click="closeMobileMenu">Projects</a>
          <a href="#github" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 py-2 border-b border-gray-700" @click="closeMobileMenu">GitHub</a>
          <a href="#contact" class="text-white hover:text-[var(--color-accent-yellow)] transition transform hover:-rotate-1 py-2" @click="closeMobileMenu">Contact</a>
        </div>
      </div>
    </header>
    
    <main class="flex-1">
      <slot />
    </main>

    <footer class="bg-gray-900 py-8 border-t-3 border-black relative">
      <div class="absolute top-0 left-0 w-16 h-16 bg-[var(--color-accent-orange)] border-black border-3 transform -rotate-12"></div>
      <div class="container mx-auto px-4 relative z-10">
        <div class="flex flex-col md:flex-row justify-between items-center">
          <div class="text-sm text-white bg-gray-800 px-4 py-2 border-black border-3 transform rotate-1 shadow-neo-sm">
            © {{ new Date().getFullYear() }} Mehdi Harzallah. All rights reserved.
          </div>
          <div class="flex space-x-4 mt-6 md:mt-0">
            <a href="https://github.com/opestro" target="_blank" rel="noopener noreferrer" 
               class="w-10 h-10 bg-white border-black border-3 flex items-center justify-center shadow-neo-sm hover:translate-y-0.5 hover:translate-x-0.5 active:translate-y-1 active:translate-x-1 active:shadow-none transition">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-black" fill="currentColor" viewBox="0 0 24 24">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
              </svg>
            </a>
            <a href="https://linkedin.com/in/mehdi-harzallah" target="_blank" rel="noopener noreferrer" 
               class="w-10 h-10 bg-[var(--color-accent-pink)] border-black border-3 flex items-center justify-center shadow-neo-sm hover:translate-y-0.5 hover:translate-x-0.5 active:translate-y-1 active:translate-x-1 active:shadow-none transition">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-white" fill="currentColor" viewBox="0 0 24 24">
                <path d="M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z"/>
              </svg>
            </a>
            <a href="mailto:mahdiharzallah21@gmail.com"
               class="w-10 h-10 bg-[var(--color-accent-yellow)] border-black border-3 flex items-center justify-center shadow-neo-sm hover:translate-y-0.5 hover:translate-x-0.5 active:translate-y-1 active:translate-x-1 active:shadow-none transition">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
              </svg>
            </a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const darkMode = ref(false);
const mobileMenuOpen = ref(false);

function toggleDarkMode() {
  darkMode.value = !darkMode.value;
  if (darkMode.value) {
    document.documentElement.classList.add('dark');
    localStorage.setItem('darkMode', 'true');
  } else {
    document.documentElement.classList.remove('dark');
    localStorage.setItem('darkMode', 'false');
  }
}

function toggleMobileMenu() {
  mobileMenuOpen.value = !mobileMenuOpen.value;
}

function closeMobileMenu() {
  mobileMenuOpen.value = false;
}

onMounted(() => {
  // Check for user preference
  const savedDarkMode = localStorage.getItem('darkMode');
  if (savedDarkMode === 'true' || (!savedDarkMode && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
    darkMode.value = true;
    document.documentElement.classList.add('dark');
  }
});
</script>

