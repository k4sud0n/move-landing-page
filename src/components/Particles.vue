<template>
    <vue-particles id="tsparticles" :options="particlesOptions" />
</template>

<script setup>
const particlesOptions = {
    background: {
        color: { value: "#000" },
    },
    fpsLimit: 60,
    interactivity: {
        events: {
            onHover: {
                enable: true,
                mode: "repulse",
            },
            resize: true,
        },
        modes: {
            repulse: {
                distance: 100,
                duration: 0.4,
            },
        },
    },
    particles: {
        color: {
            value: ["#ffffff", "#a6b8ff", "#d1aaff"], // 흰색, 푸른별, 보랏빛별
        },
        links: {
            enable: false, // 선 제거 → 더 자연스러운 우주
        },
        collisions: {
            enable: false,
        },
        move: {
            direction: "none",
            enable: true,
            speed: 0.3, // 천천히 떠다니는 별 느낌
            random: true,
            straight: false,
            outModes: {
                default: "out",
            },
        },
        number: {
            density: {
                enable: true,
                area: 1000,
            },
            value: 400,
        },
        opacity: {
            value: { min: 0.1, max: 0.5 }, // 반투명 별 느낌
        },
        shape: {
            type: ["circle", "star"], // 별과 원 섞기
        },
        size: {
            value: { min: 0.5, max: 2 },
        },
    },
    detectRetina: true,
};
</script>
