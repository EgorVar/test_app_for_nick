<script>
export default {
  data() {
    return {
      show: false
    }
  }
}

</script>

<template>
  <div class="container">
    <div class="img-wrap" v-if="show">
      <h2>Это же перцовка, которой я залью ебало Никите</h2>
      <img src="./assets/main.jpg" alt="">
      <button @click="show = false">Назад</button>
    </div>
    <div class="btn-wrap" v-else>
      <h2>Кто станет новым другом Hикиты?</h2>
      <button @click="show = true">Узнать</button>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.container{
  max-width: 600px;
  margin: 0 auto;
}
.img-wrap{
  width: 100%;
}

img{
  max-width: 88%;
}

button {
  font-size: 26px;
  margin-top: 40px;
  border: none;
  color: #fff;
  padding: 9px 27px;
  background: #8e44ad;
  border-radius: 5px;
  cursor: pointer;
}
</style>
