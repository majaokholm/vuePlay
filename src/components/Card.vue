<template>
    <div>        
        <img :src="require('@/assets/pinetrees.jpg')" alt="path fuck up" />
        <h2>Headline</h2>
        <p>Text</p>
    </div>
</template>

<script>
export default {
    name: 'card',        
}
</script>

<style scoped>
   img {
        width: 50px;
    }
</style>