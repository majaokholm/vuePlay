<template>
    <div class="rootContainer">
        <div class="imgContainer">
            <img :src='require("@/assets/logo.png")' />        
        </div>
        <div class="textContainer">           
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div>            
    </div>
</template>

<script>
export default {
    name: 'fourth-block',        
}
</script>

<style scoped>
    .rootContainer{
        display: flex;
        height: 500px;
        background-color:aqua;               
    }
    .imgContainer{        
        margin-top: 100px;
        margin-left: 300px;
    }
    .textContainer{
        margin-top: 100px;
        margin-left: 50px;
        width: 500px;
    }
</style>