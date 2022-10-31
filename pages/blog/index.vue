<template>
  <main>
    <article>
      
      <p class="mt-1 mb-4 text-primary-900">John Anthony Mallett is a graphic designer based in Te Whānganui A Tara, Wellington. They have recently completed a Bachelor of Visual Communication Design with Honours, specialising in Typographic, Digital and Print design, at Massey University College of Creative Arts Toi Rauwhārangi</p>
      <p class="mt-1 mb-4 text-primary-900">email</p>
      <p class="mt-1 mb-4 text-primary-900">email</p>


      
    </article>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, error }) {
    let posts;
    try {
      posts = await $content("blog").fetch();
    } catch (e) {
      error({ message: "Blog posts not found" });
    }
    return { posts };
  },
}
</script>
