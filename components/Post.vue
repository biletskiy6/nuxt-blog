<template>
  <article @click="goTo" class="post rounded">
    <div class="post-description">
      <h2 class="post-title mb-4">
        <n-link to="/about">About page pre-fetched</n-link>
      </h2>
      <p class="post-text mb-4">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium
        sequi corrupti molestias non recusandae amet placeat beatae, blanditiis
        dignissimos eligendi!
      </p>
      <div class="post-tags mb-2">
        <div class="post-tag text-ss rounded-full">Nuxt</div>
        <div class="post-tag text-ss rounded-full">Fetch</div>
        <div class="post-tag text-ss rounded-full">Async</div>
        <div class="post-tag text-ss rounded-full">Api</div>
      </div>

      <footer class="post-footer">
        footer
      </footer>
    </div>
    <div class="post-image">
      <img
        class="rounded"
        src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fudemy-images.udemy.com%2Fcourse%2F480x270%2F1523224_60cb.jpg&f=1&nofb=1"
        alt=""
      />
    </div>
  </article>
</template>

<script>
export default {
  methods: {
    goTo() {
      const id = "2";
      this.$router.push(`/post/${id}`);
    }
  }
};
</script>
