<template>
    <section class="text-white py-20 px-6 md:px-20 text-center mt-24">
        <h2 class="text-3xl md:text-4xl font-bold mb-12">Alumni</h2>
        <p class="text-white/70 mb-14">MOVE를 거쳐간 멋진 선배들</p>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto">
            <div
                v-for="(alumni, index) in alumniList"
                :key="index"
                class="bg-white/10 backdrop-blur-md border border-white/20 rounded-2xl p-6 hover:scale-105 transition-transform duration-300 shadow-lg"
            >
                <h3 class="text-xl font-semibold mb-2">{{ alumni.name }}</h3>
                <p class="text-sm text-white/70 mb-4">
                    {{ alumni.affiliation }}
                </p>
                <p class="italic text-white/90">“{{ alumni.quote }}”</p>
            </div>
        </div>
    </section>
</template>

<script setup>
const alumniList = [
    {
        name: "NAME TEST",
        affiliation: "소속 TEST",
        quote: "QUOTE TEST",
    },
];
</script>
