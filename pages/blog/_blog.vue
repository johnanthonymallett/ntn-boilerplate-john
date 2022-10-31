<template>
  <main>
    <section v-if="post">
      <nav class="mb-8" aria-label="go back">
        <router-back class="block" />
      </nav>

      <article>
      
        <p class="mt-1 mb-4 dark:text-gray-900">John Anthony Mallett is a graphic designer based in Te Whānganui A Tara, Wellington. They have recently completed a Bachelor of Visual Communication Design with Honours, specialising in Typographic, Digital and print design.</p>


        
      </article>
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, params, error }) {
    let post;
    try {
      post = await $content("blog", params.blog).fetch();
    } catch (e) {
      error({ message: "Blog post not found" });
    }
    return { post };
  },
  methods: {
    formatDate(dateString) {
      const date = new Date(dateString)
      return date.toLocaleDateString(process.env.lang) || ''
    }
  }
}
</script>
