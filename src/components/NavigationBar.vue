<template>
    <div class="container">        
        <p href="#" v-scroll-to="'#section-one'">First Block</p>
        <p href="#" v-scroll-to="'#section-two'">Second Block</p>
        <p href="#" v-scroll-to="'#section-three'">Third Block</p>
        <p href="#" v-scroll-to="'#section-four'">Fourth Block</p>    
    </div>
</template>

<script>
export default {
    name: 'navigation-bar',        
}
</script>

<style scoped>
    .container{
        background-color: aquamarine;
        float: left;
        width: 100%;  
        position:fixed;           
    }
    p {
        display: inline;
        margin: 10px;
    }
</style>