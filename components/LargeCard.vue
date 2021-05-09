<template>
    <NuxtLink :to="`/products/${cards.id}`" class="card">
        <img :src="require(`@/assets/images/${cards.image || 'fe1.jpg' }`)" class="image" alt="fc">
        <h3 class="header">
            {{cards.title}}
        </h3>
        <p class="snippet">
            {{cards.snippet}}
        </p>
    </NuxtLink>
</template>

<script>
    export default {
        props: ['cards'],
    }
</script>

<style scoped>
 .card {
        width: 31.5%;
        height: 25rem;
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
    }
    .image {
        height: 65%;
        border-radius: 0.5rem;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
    }
    .header {
        color: black;
        text-decoration: none;
    }
    .snippet {
        color: grey
    }
</style>