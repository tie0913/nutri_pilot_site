<script setup>
import { ArrowDownTrayIcon, DevicePhoneMobileIcon, CodeBracketIcon, VideoCameraIcon } from '@heroicons/vue/24/outline'

// TODO: 按你的实际情况改链接
const apkUrl = '#'
//'/downloads/nutripilot-alpha.apk'         // 放在 public/downloads/ 下最方便
const backendRepo = 'https://github.com/tie0913/nuitri_pilot_backend'         // 你的 repo
const frontendRepo = 'https://github.com/tie0913/nuitri_pilot_frontend'
const demoUrl = 'https://www.youtube.com/watch?v=XXXX'   // 你的 demo
const testFlightUrl = ''                                  // 有了就填，没有就留空
</script>

<template>
    <section class="py-28 bg-white px-6">
        <div class="max-w-7xl mx-auto">

            <!-- Title -->
            <div class="text-center max-w-3xl mx-auto">
                <h1 class="text-4xl md:text-5xl font-bold tracking-tight text-gray-900">
                    Download Nutri Pilot
                </h1>

            </div>

            <!-- Cards -->
            <div class="mt-16 grid md:grid-cols-2 gap-12 items-stretch">

                <!-- Android -->
                <div class="rounded-3xl border border-gray-200 p-10">
                    <div class="flex items-center gap-3">
                        <DevicePhoneMobileIcon class="w-6 h-6 text-gray-900" />
                        <h2 class="text-2xl font-semibold text-gray-900">Android (APK)</h2>
                    </div>

                    <p class="mt-4 text-gray-600 leading-relaxed">
                        Download and install the latest Android build directly on your device.
                        If Android warns about unknown sources, allow installation for this file.
                    </p>

                    <div class="mt-8">
                        <a :href="apkUrl"
                            class="inline-flex items-center gap-2 px-6 py-3 bg-green-700 hover:bg-green-900 text-white rounded-full transition-colors">
                            <ArrowDownTrayIcon class="w-5 h-5" />
                            Download APK (Comming Soon)
                        </a>
                        <p class="mt-3 text-sm text-gray-500">
                            Alpha build · Manual install
                        </p>
                    </div>
                </div>

                <!-- iOS -->
                <div class="rounded-3xl border border-gray-200 p-10">
                    <div class="flex items-center gap-3">
                        <DevicePhoneMobileIcon class="w-6 h-6 text-gray-900" />
                        <h2 class="text-2xl font-semibold text-gray-900">iOS (TestFlight)</h2>
                    </div>

                    <p class="mt-4 text-gray-600 leading-relaxed">
                        The iOS version is in progress. Once TestFlight is ready, you’ll be able to join the beta with a
                        link.
                        For now, you can still view the demo video.
                    </p>

                    <div class="mt-8">
                        <a v-if="testFlightUrl" :href="testFlightUrl" target="_blank" rel="noopener noreferrer"
                            class="inline-flex items-center gap-2 px-6 py-3 bg-gray-900 hover:bg-black text-white rounded-full transition-colors">
                            Join TestFlight
                        </a>

                        <button v-else disabled
                            class="inline-flex items-center gap-2 px-6 py-3 bg-gray-200 text-gray-500 rounded-full cursor-not-allowed">
                            TestFlight Coming Soon
                        </button>

                        <p class="mt-3 text-sm text-gray-500">
                            Beta testing · iOS review pending
                        </p>
                    </div>
                </div>
            </div>

            <!-- Resources -->
            <div class="mt-16 rounded-3xl bg-gray-50 px-10 py-12">
                <h2 class="text-3xl font-semibold text-gray-900 text-center">
                    Project Resources
                </h2>
                <p class="mt-4 text-center text-gray-600 max-w-3xl mx-auto">
                    Learn more about the implementation, architecture, and product walkthrough.
                </p>

                <div class="mt-10 flex flex-col sm:flex-row justify-center gap-4">
                    <a :href="frontendRepo" target="_blank" rel="noopener noreferrer"
                        class="inline-flex items-center justify-center gap-2 px-6 py-3 border border-gray-300 hover:border-green-800 rounded-full transition-colors">
                        <div class="flex items-center gap-3">
                            <img src="https://cdn.jsdelivr.net/npm/simple-icons@v11/icons/flutter.svg"
                                class="w-6 h-6" />
                            <span>Frontend</span>
                        </div>

                    </a>

                    <a :href="backendRepo" target="_blank" rel="noopener noreferrer"
                        class="inline-flex items-center justify-center gap-2 px-6 py-3 border border-gray-300 hover:border-green-800 rounded-full transition-colors">
                        <div class="flex items-center gap-3">
                            <img src="https://cdn.jsdelivr.net/npm/simple-icons@v11/icons/fastapi.svg"
                                class="w-6 h-6" />
                            <span>Backend</span>
                        </div>
                    </a>
                </div>
            </div>

        </div>
    </section>
</template>