<template>
<div>
    <h1 @click="indress">클릭하세요.:{{num}}</h1>
    <p v-if="num > 4">4보다 큽니다.</p>
</div>
</template>

<script>
export default {
    data(){
        return {
            num : 0
        }
    },
    methods:{
        indress(){
            this.num += 2
        }
    }
}
</script>

<style scoped>
h1{
    color:blue;
    font-size:35px;
    text-align:center;
}
p{
    font-size:35px;
    color:red;
    text-align:center;
}
</style>