<template>
    <div>
        <h1>This is project page</h1>
        <section v-if="pending">Loading...</section>
        <section v-else-if="error">Something went wrong</section>
        <section v-else>{{ data }}</section>
    </div>
</template>

<script setup>
definePageMeta({
  layout: 'app'
})
useHead({
  title:'Project'
})
const {error, pending, data} = await useFetch('https://api.github.com/users/nicorporate/repos');
// console.log(project)
</script>