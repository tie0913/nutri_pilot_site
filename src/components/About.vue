<script setup>

import tie from '@/assets/tie.jpg'
import alex from '@/assets/alex_icon.png'
import kelci from '@/assets/kelci.png'
</script>

<template>
    <section id="about" class="py-28 bg-white px-6">
        <div class="max-w-7xl mx-auto space-y-32">

            <!-- ======================= -->
            <!-- Meet the Team -->
            <!-- ======================= -->

            <div>

                <div class="text-center max-w-3xl mx-auto">
                    <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900">
                        Meet the Team
                    </h2>
                    <p class="mt-6 text-lg text-gray-600">
                        Built by a student engineering team with academic supervision.
                    </p>
                </div>

                <!-- 左右分组 -->
                <div class="mt-20 grid md:grid-cols-2 gap-20">

                    <!-- Engineering -->
                    <div>
                        <h3 class="text-2xl font-semibold text-gray-900 mb-10">
                            Engineering
                        </h3>
                        <div class="mt-10 space-y-10">
                            <div class="flex items-center gap-4">
                                <img :src="tie" alt="Tie Wang" class="w-16 h-16 rounded-full object-cover" />
                                <!-- Tie Wang -->
                                <div>
                                    <a href="https://www.linkedin.com/in/tie-wang-9b9053275/" target="_blank"
                                        rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Tie Wang
                                    </a>
                                    <p class="mt-2 text-sm text-gray-500">
                                        Full-Stack Developer · DevOps
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Faculty -->
                    <div>
                        <h3 class="text-2xl font-semibold text-gray-900 mb-10">
                            Faculty Advisors
                        </h3>
                        <div class="mt-10 space-y-10">
                            <div class="flex items-center gap-4">
                                <img :src="alex" alt="Alex Wang" class="w-16 h-16 rounded-full object-cover" />
                                <!-- Alex Wang -->
                                <div>
                                    <a href="https://www.linkedin.com/in/alex-wang-2b79593/" target="_blank"
                                        rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Alex Wang
                                    </a>

                                    <p class="mt-2 text-sm text-gray-500">
                                        Project Supervisor · Client Proxy
                                    </p>
                                </div>
                            </div>

                            <div class="flex items-center gap-4">
                                <img :src="kelci" alt="Kelci Huang" class="w-16 h-16 rounded-full object-cover" />
                                <!-- Kelci Huang -->
                                <div>
                                    <a href="https://www.linkedin.com/in/yingchao-kelci-huang-28428171/" target="_blank"
                                        rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Kelci Huang
                                    </a>

                                    <p class="mt-2 text-sm text-gray-500">
                                        Academic Advisor
                                    </p>
                                </div>
                            </div>
                        </div>

                    </div>

                </div>

            </div>

        </div>
    </section>
</template>