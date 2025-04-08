<template>
    <div class="bg-black text-white font-sans relative overflow-hidden">
        <Particles />
        <main class="relative z-10">
            <Hero />
            <AboutClub />
            <StatsPassion />
            <Features />
            <!-- <Alumni /> -->
            <WithMove />
            <MoveLinks />
            <ContactUs />
            <Footer />
        </main>
    </div>
</template>

<script setup>
import Hero from "./components/Hero.vue";
import AboutClub from "./components/AboutClub.vue";
import StatsPassion from "./components/StatsPassion.vue";
import Features from "./components/Features.vue";
import Alumni from "./components/Alumni.vue";
import WithMove from "./components/WithMove.vue";
import MoveLinks from "./components/MoveLinks.vue";
import Footer from "./components/Footer.vue";
import Particles from "./components/Particles.vue";
import ContactUs from "./components/ContactUs.vue";
</script>

<style>
body {
    margin: 0;
    font-family: "Noto Sans KR", sans-serif;
}
</style>
