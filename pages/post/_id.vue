<template>
  <div class="post-details-container">
    <n-link class="back-to font-medium v-align-center mb-10 link-hover" to="/">
      <svg
        class="icon"
        xmlns="http://www.w3.org/2000/svg"
        height="24"
        viewBox="0 0 24 24"
        width="24"
      >
        <path d="M0 0h24v24H0V0z" fill="none" />
        <path d="M15.41 7.41L14 6l-6 6 6 6 1.41-1.41L10.83 12l4.58-4.59z" />
      </svg>
      Back to blog list
    </n-link>
    <article class="post-details">
      <header>
        <h1 class="mb-4">Модуль Nuxt.js</h1>
        <div class="post-meta text-sm v-align-center">
          <div class="post-meta__author v-align-center">
            <svg class="icon" height="24" viewBox="0 0 24 24" width="24">
              <path d="M0 0h24v24H0V0z" fill="none" />
              <path
                d="M12 6c1.1 0 2 .9 2 2s-.9 2-2 2-2-.9-2-2 .9-2 2-2m0 10c2.7 0 5.8 1.29 6 2H6c.23-.72 3.31-2 6-2m0-12C9.79 4 8 5.79 8 8s1.79 4 4 4 4-1.79 4-4-1.79-4-4-4zm0 10c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"
              />
            </svg>
            <span>Victor Biletskiy</span>
          </div>
          <div class="post-meta__date">
            April 6, 2020
            <span class="dot">&#183;</span>
            17 min read
          </div>
        </div>

        <div class="mt-6">
          <img
            src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fletswrite.tw%2Fwp-content%2Fuploads%2F2019%2F12%2Fnuxt-useful-setting.jpg&f=1&nofb=1"
            alt
          />
        </div>
      </header>

      <main class="mt-12">
        <div class="excerpt">
          <em>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eaque ea, sapiente quibusdam nam natus nesciunt quaerat modi! Sit voluptatibus qui ad expedita, dolores aliquid a. Corrupti reiciendis at iste est cum iure eos voluptatem, ab nihil quaerat eum alias repellat.</em>
        </div>
        <div class="mt-12 content">
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Atque, fuga nisi reprehenderit adipisci magni enim delectus expedita harum laudantium neque!</p>
          <p>Saepe sed eum corrupti? Consectetur cum repellat eveniet explicabo minus unde, officiis, error, beatae quia consequuntur dignissimos saepe nemo. Corrupti!</p>
          <p>Blanditiis porro incidunt fugit rerum asperiores? Corporis reiciendis atque hic placeat, voluptatibus nemo animi, voluptas enim harum, laborum dignissimos maxime.</p>
          <p>Inventore possimus corrupti veniam, magnam optio omnis at minus, error facilis qui voluptates eum repellendus mollitia atque aliquid, ab voluptatibus?</p>
          <p>Voluptatum asperiores nihil unde maiores optio soluta facilis magnam laborum! Veritatis fugit, nobis mollitia nemo ex similique delectus dolor. Sit?</p>
        </div>
      </main>

      <footer>comments</footer>
    </article>

    <Comments />
  </div>
</template>

<script>
import PersonIcon from "@/assets/svg/person.svg?inline";
import Comments from "@/components/Comments";
export default {
  validate({ params }) {
    return Boolean(params.id);
  },
  components: {
    PersonIcon,
    Comments
  }
};
</script>
