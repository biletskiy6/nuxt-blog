<template>
  <div class="home-container">
    <HeroSection />
    <AppPost v-for="post in 3" :key="post" />
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import NuxtLogo from "@/assets/svg/nuxt.svg?inline";
import AppPost from "@/components/Post";
import HeroSection from "@/components/HeroSection";
export default {
  head: {
    title: "Главная"
  },
  components: {
    Logo,
    AppPost,
    NuxtLogo,
    HeroSection
  }
};
</script>
