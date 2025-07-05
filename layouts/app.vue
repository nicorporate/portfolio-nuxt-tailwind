<template>
    <div class="container mx-auto">
      <Header />
      <main class="p-2">
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
</script>

<style>
body{
  font-family: 'Roboto', sans-serif;
}
</style>