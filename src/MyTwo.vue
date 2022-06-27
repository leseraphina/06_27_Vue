<template>
<div>
    <h1 @click="str">클릭하세요 : {{num}}</h1>
    <p v-if="num > 4">4보다 큽니다.</p>
    <p v-else>4보다 작습니다.</p>
    <ul>
        <li v-for="item in colors"
            :key="item">
            {{item}}
            </li>
    </ul>
</div>
</template>
// 42
<script>
export default {
    data(){
        return {
            num : 0,
            colors:['red','blue','yellow','violet']
        }
    },
    methods:{
        str(){
            this.num += 1;
        }
    }
}
</script>

<style scoped>
div{text-align:center;}
 h1{ font-size:50px; color:red;}
 p{font-size:50px; color:green;}
 ul,li{list-style-type:none;}
 ul{
    background-color:#666;
    color:#fff;
 }
</style>