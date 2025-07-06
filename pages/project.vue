<template>
    <div>
        <h1>This is project page</h1>
    </div>
</template>

<script setup>
definePageMeta({
  layout: 'app'
})
useHead({
  title:'Project'
})
const project = await $fetch('https://api.github.com/users/nicorporate/repos');
console.log(project)
</script>