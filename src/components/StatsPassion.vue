<template>
    <section class="bg-black text-white py-16 px-6 md:px-20 text-center mt-40">
        <h2 class="text-3xl md:text-4xl font-bold mb-12">
            숫자가 말해주는 우리의 열정
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
            <div
                class="border border-white/20 rounded-2xl p-8 hover:scale-105 transition transform duration-300 shadow-lg"
            >
                <p class="text-5xl font-extrabold text-indigo-400">
                    <AnimatedCounter
                        :value="34"
                        :duration="1000"
                        class="counter"
                    />
                </p>
                <p class="mt-2 text-lg">활동 중인 멤버</p>
            </div>

            <div
                class="border border-white/20 rounded-2xl p-8 hover:scale-105 transition transform duration-300 shadow-lg"
            >
                <p class="text-5xl font-extrabold text-pink-400">
                    <AnimatedCounter
                        :value="20"
                        :duration="1000"
                        class="counter"
                    />
                </p>
                <p class="mt-2 text-lg">진행한 프로젝트</p>
            </div>

            <div
                class="border border-white/20 rounded-2xl p-8 hover:scale-105 transition transform duration-300 shadow-lg"
            >
                <p class="text-5xl font-extrabold text-yellow-400">100%</p>
                <p class="mt-2 text-lg">만족도</p>
            </div>

            <div
                class="border border-white/20 rounded-2xl p-8 hover:scale-105 transition transform duration-300 shadow-lg"
            >
                <p class="text-5xl font-extrabold text-green-400">
                    <AnimatedCounter
                        :value="50"
                        :duration="1000"
                        class="counter"
                    />
                </p>
                <p class="mt-2 text-lg">정기 세션 개최</p>
            </div>

            <div
                class="border border-white/20 rounded-2xl p-8 hover:scale-105 transition transform duration-300 shadow-lg"
            >
                <p class="text-5xl font-extrabold text-cyan-400">24시간</p>
                <p class="mt-2 text-lg">불타는 열정</p>
            </div>

            <div
                class="border border-white/20 rounded-2xl p-8 hover:scale-105 transition transform duration-300 shadow-lg"
            >
                <p class="text-5xl font-extrabold text-red-400">1</p>
                <p class="mt-2 text-lg">단 하나뿐인 팀워크</p>
            </div>
        </div>
    </section>
</template>

<script setup>
import AnimatedCounter from "vue-animated-counter";
</script>
