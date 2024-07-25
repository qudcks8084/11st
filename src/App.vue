<template>
  <div class="menu">
    <a v-for="(eachmenu,index) in menubar" :key="index">{{eachmenu}} </a>
  </div>

  <div v-for="(eachData, index) in product" :key="index">
    <h4>{{eachData.name}}</h4> 
    <p>{{eachData.price}} 만원</p>
    <button v-on:click="increase(eachData)">허위매물신고</button> <span>신고수 : {{ eachData.click }}</span>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){ // 데이터 보관
    return{
      menubar : ['Home', 'Product', 'About'],
      product : [
        {name : '역삼동원룸', price : 10, click : 0},
        {name : '천호동원룸', price : 20, click : 0},
        {name : '마포구원룸', price : 30, click : 0}
      ],
    }
  },

  methods : {
    increase(eachData){
      eachData.click +=1 ;
    }
  },
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.menu {
  background: darkslateblue;
  padding : 15px;
  border-radius: 5px;
}

.menu a{
  color: white;
  padding: 10px;
}
</style>
