<script setup>
import logo from '@/assets/vite-cropped.svg'
import { ref } from 'vue'
import { BarsArrowUpIcon, BarsArrowDownIcon } from '@heroicons/vue/24/outline'
const open = ref(false)
</script>
<template>
  <header class="sticky top-0 bg-white z-50 bg-white/80 backdrop-blur border-b border-green-800">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <!-- Logo 区 -->
      <div class="flex items-center gap-3">
        <!-- 你的Logo放这里 -->
        <img :src="logo" alt="Nutri Pilot" class="w-8 h-8" />
        <span class="hidden md:block font-semibold text-lg">
          Nutri <span class="text-green-700">Pilot</span>
        </span>
      </div>

      <!-- 导航 -->
      <nav class="hidden md:flex gap-8 text-gray-600">
        <a href="#hero" class="hover:text-black">Home</a>
        <a href="#features" class="hover:text-black">Features</a>
        <a href="#download" class="hover:text-black">Download</a>
        <a href="#about" class="hover:text-black">About</a>
      </nav>

      <button @click="open = !open" class="md:hidden text-2xl">
        <BarsArrowDownIcon v-if="!open" class="w-6 h-6 text-gray-800"></BarsArrowDownIcon>
        <BarsArrowUpIcon v-if="open" class="w-6 h-6 text-gray-800"></BarsArrowUpIcon>
      </button>
    </div>
    <div v-if="open" class="md:hidden absolute text-center top-full w-full bg-gray-100 border-t">
      <a href="#hero" class="block text-green-900" @click="open=false">Home</a>
      <a href="#features" class="block text-green-900" @click="open=false">Features</a>
      <a href="#download" class="block text-green-900" @click="open=false">Demo</a>
      <a href="#about" class="block text-green-900" @click="open=false">About</a>
    </div>
  </header>


</template>