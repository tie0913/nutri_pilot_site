<script setup>
import app from '@/assets/app.png'
import { InformationCircleIcon, ArrowDownCircleIcon} from '@heroicons/vue/24/outline';
</script>
<template>
    <section id="hero" class="min-h-screen flex items-center bg-white px-6">
        <div class="max-w-7xl mx-auto grid md:grid-cols-2 gap-12 items-center">
            <!-- 左侧文字 -->
            <div class="text-center md:text-left">

                <h1 class="text-5xl md:text-6xl font-bold tracking-tight text-gray-900">
                    Nutri <span class="text-green-700">Pilot</span>
                </h1>

                <p class="mt-6 text-xl text-gray-600">
                    Intelligent Nutrition Guidance powered by AI
                </p>

                <p class="mt-4 text-gray-500">
                    Analyze food safety based on your health conditions,
                    allergies, and dietary restrictions.
                </p>

                <div class="mt-8 flex justify-center md:justify-start gap-4">
                   
                    <a href="#features" class="px-6 py-3 bg-green-700 hover:bg-green-900 text-white rounded-full transition cursor-pointer flex items-center gap-2">
                        <InformationCircleIcon class="w-6 h-6"/>
                        <span class="">Learn More</span>
                    </a>
                    <a href="#download" class="px-6 py-3 border border-gray-400 hover:border-green-800 rounded-full cursor-pointer flex item-center gap-2">
                        <ArrowDownCircleIcon class="w-6 h-6"/>
                      Download
                    </a>
                </div>
            </div>

            <!-- 右侧手机截图区域 -->
            <div class="flex justify-center">
                <div class="w-[260px] md:w-[320px] aspect-[9/19.5] bg-gray-200 rounded-[2rem] overflow-hidden shadow-2xl flex items-center justify-center">
                    <!--
                    <img :src="app" class="w-full h-full object-cover "/>
                    -->
                    <iframe class="w-full h-full" src="https://player.vimeo.com/video/1171169957?h=6ba992cae4" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe>
                </div>
            </div>

        </div>
    </section>


</template>