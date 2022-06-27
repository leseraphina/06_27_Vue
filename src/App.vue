<template>
  <div>
    <h1 @click="incress">클릭하세요.</h1>
    <p>{{count}}</p>
  </div>
</template>

<script>
export default {
  data(){
    return {
      count : 0
    }
  },
  methods:{
    incress(){
      this.count += 3;
    }
  }
}
</script>
//  스타일 이 지역적으로
<style scoped>
h1{
  font-size:50px;
  color:green;
  text-align:center;
}
p{
  font-size:25px;
  color:red;
  text-align:center;
}
</style>