<template>
  <main class="bg-gradient-to-r ">
    <header class="flex items-center justify-between px-8 py-4 max-w-7xl mx-auto shadow-sm relative">
      <div class="flex items-center space-x-2">
        <img src="@/assets/img/transparent2.png" alt="" class="h-20 w-20" />
      </div>
      <div class="md:hidden">
        <button @click="toggleMenu" class="focus:outline-none">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
        </button>
      </div>
      <nav class="hidden md:flex space-x-8">
        <a href="www.mentor-techies.com" class="text-white hover:text-blue-500 transition-colors">For Mentorship</a>
        <a href="https://www.enforcatech.com/mentee/login" class="text-white hover:text-blue-500 transition-colors">For Job seekers</a>
      </nav>
      <a href="www.mentor-techies.com" class="hidden md:block bg-[#111D63] text-white py-3 text-sm px-4 rounded-full shadow-md hover:bg-blue-800 transition-colors">
        Get Started
      </a>
    </header>
    <div v-if="isMenuOpen" class="absolute top-16 left-0 w-screen z-50 md:hidden">
      <nav class="flex flex-col space-y-4 bg-white p-4 shadow-lg rounded-b-lg">
        <NuxtLink to="" @click="closeMenu" class="text-[#000316] hover:text-blue-500 transition-colors">Mentorship</NuxtLink>
        <a ref="www.mentor-techies.com"  @click="closeMenu" class="text-[#000316] hover:text-blue-500 transition-colors">Need AI job application and support </a>
        <a href="www.mentor-techies.com" @click.native="closeMenu" class="bg-[#111D63] text-white py-3 text-sm px-4 rounded-full shadow-md hover:bg-blue-800 transition-colors">
          Get Started
        </a>
      </nav>
    </div>
  </main>
</template>

<script setup lang="ts">
import { ref } from 'vue';

// State to control the mobile menu visibility
const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

const closeMenu = () => {
  isMenuOpen.value = false;
};
</script>

<style scoped>
/* Add any specific styles here */
</style>
