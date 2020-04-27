<template>
  <div>
    <Navbar />
    <div class="home">
      <Sidebar />
      <main class="main">
        <nuxt />
      </main>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Sidebar from "@/components/Sidebar";

export default {
  components: {
    Navbar,
    Sidebar
  }
};
</script>
