<script setup>

import tie from '@/assets/tie.jpg'
import smit from '@/assets/smit.jpg'
import nihar from '@/assets/nihar.jpg'

</script>

<template>
    <section class="py-28 bg-white px-6">
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
                            Engineering Team
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
                                        System Architect · Full-Stack Developer · DevOps
                                    </p>
                                </div>
                            </div>

                            <div class="flex items-center gap-4">
                                <!-- Dhruv Patel -->
                                <div>
                                    <a href="#" target="_blank" rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Dhruv Patel
                                    </a>
                                    <p class="mt-2 text-sm text-gray-500">
                                        Tester
                                    </p>
                                </div>
                            </div>
                            <div class="flex items-center gap-4">
                                <img :src="nihar" alt="Nihar Parekh" class="w-16 h-16 rounded-full object-cover" />
                                <!-- Nihar Parekh -->
                                <div>
                                    <a href="https://www.linkedin.com/in/nihar-parekh-3088a6239/" target="_blank"
                                        rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Nihar Parekh
                                    </a>
                                    <p class="mt-2 text-sm text-gray-500">
                                        Tester
                                    </p>
                                </div>
                            </div>

                            <div class="flex items-center gap-4">
                                <img :src="smit" alt="Smit Ashwinbhai Parmar"
                                    class="w-16 h-16 rounded-full object-cover" />
                                <!-- Smit -->
                                <div>
                                    <a href="https://www.linkedin.com/in/smit-parmar-745a89363/" target="_blank"
                                        rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Smit Ashwinbhai Parmar
                                    </a>
                                    <p class="mt-2 text-sm text-gray-500">
                                        UI Designer
                                    </p>
                                </div>
                            </div>
                            <div class="flex items-center gap-4">
                                <!-- Ayra Bharatbhai Patel -->
                                <div>
                                    <a href="#" target="_blank" rel="noopener noreferrer"
                                        class="text-xl font-semibold text-gray-900 hover:text-green-700 transition-colors duration-200">
                                        Ayra Bharatbhai Patel
                                    </a>
                                    <p class="mt-2 text-sm text-gray-500">
                                        UI Designer
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


            <!-- ======================= -->
            <!-- Technical Architecture -->
            <!-- ======================= -->
            <div class="py-24 bg-gray-50 px-10 rounded-3xl">

                <!-- Title -->
                <div class="text-center max-w-3xl mx-auto">
                    <h2 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900">
                        Technical Architecture
                    </h2>

                    <p class="mt-6 text-lg text-gray-600">
                        Nutri Pilot is built as a modular full-stack AI platform designed for scalability and real-time
                        food analysis.
                    </p>
                </div>

                <!-- Architecture Columns -->
                <div class="mt-20 grid md:grid-cols-3 gap-16">

                    <!-- Frontend -->
                    <div>
                        <h3 class="text-xl font-semibold text-gray-900">
                            Frontend
                        </h3>

                        <ul class="mt-6 space-y-3 text-gray-600 leading-relaxed">
                            <li>Flutter cross-platform mobile application</li>
                            <li>Vue 3 + Tailwind landing website</li>
                            <li>Component-based UI architecture</li>
                        </ul>
                    </div>

                    <!-- Backend -->
                    <div>
                        <h3 class="text-xl font-semibold text-gray-900">
                            Backend
                        </h3>

                        <ul class="mt-6 space-y-3 text-gray-600 leading-relaxed">
                            <li>FastAPI asynchronous REST API</li>
                            <li>Python AI image analysis pipeline</li>
                            <li>Request validation & rate limiting</li>
                            <li>Scalable service architecture</li>
                        </ul>
                    </div>

                    <!-- Infrastructure -->
                    <div>
                        <h3 class="text-xl font-semibold text-gray-900">
                            Infrastructure
                        </h3>

                        <ul class="mt-6 space-y-3 text-gray-600 leading-relaxed">
                            <li>Gpt-4o-mini integeration</li>
                            <li>Cloudflare R2 object storage</li>
                            <li>Persistent database storage</li>
                            <li>RESTful API communication</li>
                            <li>Container-ready deployment</li>
                        </ul>
                    </div>

                </div>

            </div>

        </div>
    </section>
</template>