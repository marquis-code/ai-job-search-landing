<!-- 
<template>
    <div class="bg-gray-100 py-16">
      <h2 class="text-center text-2xl md:text-4xl font-bold mb-8">
        2
      </h2>
      <div class="flex flex-wrap justify-center items-start gap-8 max-w-4xl mx-auto">
        <div class="w-64 text-center p-4 bg-white rounded shadow-lg" v-for="(step, index) in steps" :key="index">
          <div class="w-16 h-16 mx-auto bg-blue-500 rounded-full flex items-center justify-center text-white mb-4">
            <img :src="step.icon" alt="step icon" class="w-8 h-8">
          </div>
          <h3 class="font-bold text-lg">{{ step.title }}</h3>
          <p class="mt-2 text-gray-500">{{ step.description }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  const steps = [
    {
      icon: '/path/to/icon1.png',
      title: 'Get Career Roadmap',
      description: 'Upload your CV for review analysis and initial feedback on key skills and experience.'
    },
    {
      icon: '/path/to/icon2.png',
      title: 'Get real experience with expert guidance',
      description: 'We take you into the real world of how to do in your chosen career beyond the theory knowledge.'
    },
    {
      icon: '/path/to/icon3.png',
      title: 'Simulated Interview Session',
      description: 'Practice answering both behavioral and technical interview questions in a safe and supportive environment.'
    },
    {
      icon: '/path/to/icon4.png',
      title: 'Land the Job',
      description: 'Track your job applications and schedule interviews with ease using our automated and streamlined platform.'
    },
  ];
  </script>
   -->
<!-- 
  <template>
    <div class="bg-gray-50">
        <h2 class="text-center text-2xl md:text-4xl font-bold mb-8">
            Unleash your full potential and land your dream job in 4 easy steps
          </h2>
      <div class="mx-auto max-w-2xl px-4 py-24 sm:px-6 sm:py-32 lg:max-w-7xl lg:px-8">
        <div class="grid grid-cols-1 gap-y-12 sm:grid-cols-2 sm:gap-x-6 lg:grid-cols-4 lg:gap-x-8">
          <div v-for="incentive in incentives" :key="incentive.name">
            <img :src="incentive.imageSrc" alt="" class="h-24 w-auto" />
            <h3 class="mt-6 text-sm font-medium text-gray-900">{{ incentive.name }}</h3>
            <p class="mt-2 text-sm text-gray-500">{{ incentive.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const incentives = [
    {
      name:  'Get Career Roadmap',
      description: 'Upload your CV for review analysis and initial feedback on key skills and experience.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-delivery-light.svg',
    },
    {
      name: 'Get real experience with expert guidance',
      description: 'We take you into the real world of how to do in your chosen career beyond the theory knowledge.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-chat-light.svg',
    },
    {
      name: 'Simulated Interview Session',
      description: 'Practice answering both behavioral and technical interview questions in a safe and supportive environment.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-fast-checkout-light.svg',
    },
    {
      name: 'Land the Job',
      description: 'Track your job applications and schedule interviews with ease using our automated and streamlined platform.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-gift-card-light.svg',
    },
  ]
  </script> -->

<template>
    <div class="bg-white">
      <div class="mx-auto max-w-7xl py-24 sm:px-2 sm:py-32 lg:px-4">
        <div class="mx-auto max-w-2xl px-4 lg:max-w-none">
          <div class="max-w-3xl">
            <h2 class="text-4xl font-bold tracking-tight text-gray-900">We built our business on customer service</h2>
            <!-- <p class="mt-4 text-gray-500">At the beginning at least, but then we realized we could make a lot more money if we kinda stopped caring about that. Our new strategy is to write a bunch of things that look really good in the headlines, then clarify in the small print but hope people don't actually read it.</p> -->
          </div>
          <div class="mt-16 grid grid-cols-1 gap-x-8 gap-y-10 lg:grid-cols-3">
            <div v-for="incentive in incentives" :key="incentive.name" class="sm:flex lg:block">
              <div class="sm:flex-shrink-0">
                <img class="h-16 w-16" :src="incentive.imageSrc" alt="" />
              </div>
              <div class="mt-4 sm:ml-6 sm:mt-0 lg:ml-0 lg:mt-6">
                <h3 class="text- font-medium text-gray-900">{{ incentive.name }}</h3>
                <p class="mt-2 text- text-gray-500">{{ incentive.description }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const incentives = [
    {
      name:  'Get Career Roadmap',
      description: 'Upload your CV for review analysis and initial feedback on key skills and experience.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-delivery-light.svg',
    },
    {
      name: 'Get real experience with expert guidance',
      description: 'We take you into the real world of how to do in your chosen career beyond the theory knowledge.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-chat-light.svg',
    },
    {
      name: 'Simulated Interview Session',
      description: 'Practice answering both behavioral and technical interview questions in a safe and supportive environment.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-fast-checkout-light.svg',
    },
    {
      name: 'Land the Job',
      description: 'Track your job applications and schedule interviews with ease using our automated and streamlined platform.',
      imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-gift-card-light.svg',
    },
  ]
  </script>