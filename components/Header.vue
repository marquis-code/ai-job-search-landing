<template>
  <main class="bg-gradient-to-r from-white to-blue-50">
    <header class="flex items-center justify-between px-8 py-4 max-w-7xl mx-auto shadow-sm relative">
      <!-- Logo Section -->
      <div class="flex items-center space-x-2">
        <img src="@/assets/icons/logo.svg" alt="GetreKruitd Logo" class="h-8" />
      </div>

      <!-- Hamburger Menu for Mobile -->
      <div class="md:hidden">
        <button @click="toggleMenu" class="focus:outline-none">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
          </svg>
        </button>
      </div>

      <!-- Navigation Links -->
      <nav class="hidden md:flex space-x-8">
        <a href="#" class="text-[#000316] hover:text-blue-500 transition-colors">Schedule Consultation</a>
        <a href="#" class="text-[#000316] hover:text-blue-500 transition-colors">Review Resume</a>
      </nav>

      <!-- Dashboard Button -->
      <button class="hidden md:block bg-[#111D63] text-white py-3 text-sm px-4 rounded-full shadow-md hover:bg-blue-800 transition-colors">
        My Dashboard
      </button>
    </header>

    <!-- Mobile Dropdown Menu -->
    <div v-if="isMenuOpen" class="absolute top-16 left-0 w-screen z-50 md:hidden">
      <nav class="flex flex-col space-y-4 bg-white p-4 shadow-lg rounded-b-lg">
        <a href="#" @click="closeMenu" class="text-[#000316] hover:text-blue-500 transition-colors">Schedule Consultation</a>
        <a href="#" @click="closeMenu" class="text-[#000316] hover:text-blue-500 transition-colors">Review Resume</a>
        <button @click="closeMenu" class="bg-[#111D63] text-white py-3 text-sm px-4 rounded-full shadow-md hover:bg-blue-800 transition-colors">
          My Dashboard
        </button>
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
