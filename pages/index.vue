<template>
  <div :style="backgroundStyle" class="min-h-screen">
    <Header />
    <MainContent />
    <Footer />
  </div>
</template>

<script setup lang="ts">
import { useHead } from '@vueuse/head';
import Header from '~/components/Header.vue';
import MainContent from '~/components/MainContent.vue';
const background1 = new URL('@/assets/img/landing1.jpg', import.meta.url).href;
const backgroundStyle = {
  backgroundImage: `url(${background1})`, // or use background2 if needed
  backgroundSize: 'cover',
  backgroundPosition: 'center',
};

useHead({
  title: 'GetreKruitd - AI-Powered Job Processing Platform',
  meta: [
    {
      name: 'description',
      content: 'GetreKruitd is an AI-Powered Job Processing Platform that guides you through ATS processes, pairs you with industry mentors, and advises on continuous skill development.',
    },
    {
      name: 'keywords',
      content: 'AI, Job Processing, ATS, Industry Mentors, Skill Development, GetreKruitd',
    },
    {
      property: 'og:title',
      content: 'GetreKruitd - AI-Powered Job Processing Platform',
    },
    {
      property: 'og:description',
      content: 'GetreKruitd is an AI-Powered Job Processing Platform that guides you through ATS processes, pairs you with industry mentors, and advises on continuous skill development.',
    },
    {
      property: 'og:image',
      content: 'https://example.com/path/to/your/image.jpg',
    },
    {
      property: 'og:url',
      content: 'https://www.enforcatech.com/',
    },
    {
      name: 'twitter:card',
      content: 'summary_large_image',
    },
    {
      name: 'twitter:title',
      content: 'GetreKruitd - AI-Powered Job Processing Platform',
    },
    {
      name: 'twitter:description',
      content: 'GetreKruitd is an AI-Powered Job Processing Platform that guides you through ATS processes, pairs you with industry mentors, and advises on continuous skill development.',
    },
    {
      name: 'twitter:image',
      content: 'https://example.com/path/to/your/image.jpg',
    },
  ],
});
</script>

<style>
/* Add any global styles here */
</style>
