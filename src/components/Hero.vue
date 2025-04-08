<template>
    <section
        class="min-h-screen flex flex-col justify-center items-center text-center px-6"
        data-aos="fade-up"
    >
        <h1 class="text-4xl md:text-6xl font-bold mb-4">
            HUFS_
            <VueWriter
                :array="['HUVE', 'SPRINT', 'MOVE']"
                :eraseSpeed="100"
                :typeSpeed="150"
                :delay="2000"
                :caret="cursor"
            />
        </h1>
        <p class="text-lg md:text-xl mb-6 max-w-2xl">
            세상을 변화시킬 그 원대한 시작, <br />
            우리들의 도전이 세상을 변화시킨다.
        </p>
        <a href="https://forms.gle/MWEi8PbUnwwxCMKo7" target="_blank">
            <button
                class="bg-white text-black px-6 py-3 rounded-full font-semibold hover:bg-gray-300 transition"
            >
                지금 함께하기
            </button>
        </a>
    </section>
</template>

<script setup>
import { VueWriter } from "vue-writer";
</script>
