<template>
    <div>
        <h1>This is {{ route.params.id }} page</h1>
    </div>
</template>

<script setup>

const route = useRoute();
console.log(route)

</script>