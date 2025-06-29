<template>
  <div id="app">
    <HeroSection />
    <CareerSection />
    <ContactSection />
  </div>
</template>

<script setup>
import HeroSection from './components/HeroSection.vue'
import CareerSection from './components/CareerSection.vue'
import ContactSection from './components/ContactSection.vue'
</script>

<style>
/* 기본 스타일 초기화 */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', 'Noto Sans KR', sans-serif;
  background-color: #fdfdfd;
  color: #222;
  scroll-behavior: smooth;
}

#app {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}
</style>
