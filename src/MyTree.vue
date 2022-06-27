<template>
    <ul>
        <hellow-app
            v-for="item in colors"
            :key="item"
            :name="item">
            {{item}}
        </hellow-app>
    </ul>
</template>

<script>
import HellowApp from './components/HellowApp.vue'
export default {
    components:{HellowApp},
    data(){
        return {
            colors:['red','blue','yellow','violet']
        }
        
    },
    methods:{}
}
</script>

<style scoped>
 ul>li{
    font-size:40px;
    color:pink;
 }
</style>