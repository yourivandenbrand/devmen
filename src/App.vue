<template>
  <div id="app" class="container-fluid">
    <hero></hero>
    <join></join>
    <team></team>
    <clients></clients>
    <!-- <footer></footer> -->
  </div>
</template>

<script>
import Hero from "./site/Hero.vue"
import Join from "./site/Join.vue"
import Team from "./site/Team.vue"
import Clients from "./site/Clients.vue"

export default {
  name: 'app',
  components:{
    Hero, Join, Team, Clients
  }
}
</script>

<style>
#app {
  text-align: center;
  color: #2c3e50;
}

.theme-yellow{
  background-color:#fbe108;
  color:#000;
}

.theme-grey{
  background-color: #efefef;
  color: #000;
}

.content{
    padding-top: 3em;
    padding-bottom: 3em;
    text-align: left;
}
</style>
