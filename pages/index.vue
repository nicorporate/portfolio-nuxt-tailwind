<template>
    <div>
        <h1>Nuxt Routing set up successfully</h1>
        <p>Current route: {{ route.path }}</p>
        <a href=""></a>
    </div>
</template>

<script setup lang="ts">

const route = useRoute()

</script>