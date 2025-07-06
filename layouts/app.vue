<template>
    <div class="container mx-auto">
      <Header />
      <main class="p-2 mt-10">
        <slot />
      </main>
    </div>
</template>


<script setup>
useHead({
  titleTemplate:'%s - Porto',
  link: [
    {
      rel:"preconnect",
      href:"https://fonts.googleapis.com"
    },
    {
      rel:"stylesheet",
      href:"https://fonts.googleapis.com/css2?family:Roboto:ital,wght@0,100..900;1,100..900&display=swap", 
      crossorigin:"anonymous"
    },
  ]
})
useSeoMeta({
  title: 'My Portfolio',
  description: 'This is my amazing site, let me tell you all about it.',
  ogTitle: 'My Portfolio',
  ogDescription: 'This is my amazing site, let me tell you all about it.',
  ogImage: 'https://example.com/image.png',
  twitterCard: 'summary_large_image',
  twitterTitle: 'My Portfolio',
  twitterDescription: 'This is my amazing site, let me tell you all about it.'
})
</script>

<style>
body{
  font-family: 'Roboto', sans-serif;
}
</style>