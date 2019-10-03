<template>
    <div class="rootContainer">
        <div class="smallContainer">
            <card/>        
        </div>
        <div class="smallContainer">
            <card/>        
        </div>
        <div class="smallContainer">
            <card/>    
        </div>        
    </div>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
    name: 'second-block',
    components: {
        Card,
    }
    
}
</script>

<style scoped>
    .rootContainer{
        height: 500px;
        background-color: aquamarine;               
    }
    .smallContainer{
        display: inline-block;
        margin-top: 100px;  
        margin-right: 10px;        
        margin-left: 10px;
    }
</style>