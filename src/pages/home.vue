<template>
    <div class="home">
       <Index/>
    </div>
</template>
<script>
// import index from '@/pages/index/index.vue'
import Index from './index/index.vue'
export default {
    name:'home',
    data(){
        return{

        }
    },
    components:{
        Index,
    }
}
</script>

<style scoped>
.home{
    border-top: 1px solid #D8D8D8; 
    border-top-width: 100%;
    border-bottom-width: 100%;
    width: 1190px;
    height: 80px;
    margin-top: 0;
    padding-left: 0;
    margin-left: auto;
    margin-right: auto;
    border-bottom: 1px solid #D8D8D8;
}
</style>