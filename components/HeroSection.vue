<template>
  <div class="hero-section">
    <div class="hero-section__description">
      <h1 class="mb-6"><span>&lt;V.B&gt;</span> Blog</h1>
      <p>
        Откройте для себя статьи основной команды и авторов о NuxtJS, советы и
        хитрости в том числе!
      </p>
    </div>

    <div class="hero-section__image">
      <HeroSvg />
    </div>
  </div>
</template>

<script>
import HeroSvg from "@/assets/svg/nuxt.svg?inline";

export default {
  components: {
    HeroSvg
  }
};
</script>
