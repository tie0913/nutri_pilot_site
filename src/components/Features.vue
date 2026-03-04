<script setup>
import feedback from '@/assets/ai-feedback.png'
</script>

<template>
  <section id="features" class="py-24 bg-white px-6">
    <div class="max-w-7xl mx-auto grid md:grid-cols-2 gap-12 items-center">

      <!-- 左侧文字 -->
      <div class="text-center md:text-left">

        <!-- 主标题（比 Hero 小一档） -->
         <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900 max-w-xl">
          AI that understands <br class="hidden md:block" />your health.
        </h2>

        <!-- 副标题 -->
        <p class="mt-6 text-lg text-gray-600">
          <span class="text-green-700">Nutri Pilot</span> evaluates food based on your allergies,
          chronic conditions, and nutritional goals.
        </p>

        <!-- Feature 列表 -->
        <div class="mt-10 space-y-8">

          <div>
            <h3 class="text-xl font-semibold text-gray-900">
              Personalized Risk Scoring
            </h3>
            <p class="mt-2 text-base text-gray-500">
              Every meal is evaluated based on your specific health profile,
              not generic nutrition standards.
            </p>
          </div>

          <div>
            <h3 class="text-xl font-semibold text-gray-900">
              AI-Powered Explanations
            </h3>
            <p class="mt-2 text-base text-gray-500">
              Understand why a food is suitable — or risky — for your
              condition with clear, transparent feedback.
            </p>
          </div>

          <div>
            <h3 class="text-xl font-semibold text-gray-900">
              Smart Recommendations
            </h3>
            <p class="mt-2 text-base text-gray-500">
              Get tailored suggestions when a meal isn’t ideal,
              helping you make better decisions instantly.
            </p>
          </div>

        </div>

      </div>

      <!-- 右侧图片（比例与 Hero 一致） -->
      <div class="flex justify-center">
        <div class="w-[260px] md:w-[320px] rounded-[2rem] overflow-hidden shadow-2xl">
          <img
            :src="feedback"
            alt="AI feedback preview"
            class="w-full h-full object-cover"
          />
        </div>
      </div>

    </div>
  </section>
</template>