<template>
  <main>
    <article>
      <h2 class="mt-4 mb-4 subtitle">John Anthony Mallett</h2>
      <p class="mt-1 mb-6 text-primary-900">Graphic designer based in Te Whānganui A Tara, Wellington. They have recently completed a Bachelor of Visual Communication Design with Honours, specialising in Typographic, Digital and Print design, at Massey University College of Creative Arts Toi Rauwhārangi</p>
      <p class="mt-1 mb-4 text-primary-900">email:</p>
      <p class="mt-1 mb-4 text-primary-900"><a href="mailto:johnanthonymallett@gmail.com">johnanthonymallett@gmail.com</a></p>
      <p class="mt-1 mb-10 text-primary-900"><a href="https://www.are.na/john-mallett">are.na</a></p>

      <h2 class="mt-8 mb-4 subtitle">Experience</h2>

      <p class="mt-1 mb-1 text-primary-900">2019&#x200D;&#x200A;&#x200D;—&#x200D;&#x200A;&#x200D;2022</p>      
      <p class="mt-1 mb-0 text-primary-900"><a href="https://creative.massey.ac.nz/">Massey University College of Creative Arts Toi Rauwhārangi</a></p>
      <p class="mt-1 mb-4 text-primary-900">Bachelor of Visual Comunication Design with Honours</p>

      <p class="mt-1 mb-1 text-primary-900">2022&#x200D;&#x200A;&#x200D;—&#x200D;&#x200A;&#x200D;present</p>
      <p class="mt-1 mb-0 text-primary-900"><a href="https://effect.nz/">Effect</a></p>
      <p class="mt-1 mb-4 text-primary-900">Junior Designer</p>

      <p class="mt-1 mb-1 text-primary-900">2021</p>
      <p class="mt-1 mb-0 text-primary-900"><a href="https://bestawards.co.nz/graphic/student-graphics/massey-university-college-of-creative-arts/20-fonts-that-changed-the-world/">DINZ Best Awards</a></p>
      <p class="mt-1 mb-4 text-primary-900">Bronze&#x200D;&#x200A;&#x200D;—&#x200D;&#x200A;&#x200D;Student Graphics</p>
      


      
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
