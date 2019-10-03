<template>
    <div>
        <h1>test</h1>
        <img :src='require("@/assets/logo.png")' />
        <h1>test</h1>
        <img :src='require("@/assets/logo.png")' />
        <h1>test</h1>
        <img :src='require("@/assets/logo.png")' />
    </div>
</template>

<script>
export default {
    name: 'home',    
    methods: {
        scroll(){

        }
    }
}
</script>

<style scoped>
    img {
        background-color: aqua;
    }
</style>