<script setup>
import logo from '@/assets/vite-cropped.svg'
import {ref} from 'vue'
import {BarsArrowUpIcon, BarsArrowDownIcon} from '@heroicons/vue/24/outline'
const open=ref(false)

</script>
<template>
<header class="sticky top-0 bg-white z-50 bg-white/80 backdrop-blur border-b border-green-800">
  <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
    <!-- Logo 区 -->
    <div class="flex items-center gap-3">
      <!-- 你的Logo放这里 -->
       <img :src="logo" alt="Nutri Pilot" class="w-8 h-8"/>
       <span class="hidden md:block font-semibold text-lg">
          Nutri <span class="text-green-700">Pilot</span>
        </span>
    </div>

    <!-- 导航 -->
    <nav class="hidden md:flex gap-8 text-gray-600">
      <a href="#" class="hover:text-black">Home</a>
      <a href="#" class="hover:text-black">Features</a>
      <a href="#" class="hover:text-black">Download</a>
      <a href="#" class="hover:text-black">About</a>
    </nav>

    <button @click="open = !open" class="md:hidden text-2xl">
      <BarsArrowDownIcon v-if="!open" class="w-6 h-6 text-gray-800"></BarsArrowDownIcon>
      <BarsArrowUpIcon v-if="open" class="w-6 h-6 text-gray-800"></BarsArrowUpIcon>
    </button>
  </div>
</header>

<div v-if="open" class="md:hidden px-4 pb-4 space-y-2 bg-gray-100 text-center">
  <a class="block text-green-900">Home</a>
  <a class="block text-green-900">Features</a>
  <a class="block text-green-900">Demo</a>
  <a class="block text-green-900">About</a>
</div>

</template>