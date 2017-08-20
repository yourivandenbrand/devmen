<template>
  <div id="app">
    <hero></hero>
    <join></join>
    <team></team>
    <clients></clients>
    <foot></foot>
  </div>
</template>

<script>
import Hero from "./components/Hero.vue"
import Join from "./components/Join.vue"
import Team from "./components/Team.vue"
import Clients from "./components/Clients.vue"
import Foot from "./components/Foot.vue"

export default {
  name: 'app',
  components:{
    Hero, Join, Team, Clients, Foot
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

.theme-black{
  background-color: #000;
  color: #fff;
}

.content{
    padding-top: 3em;
    padding-bottom: 3em;
    text-align: left;
}

a,
a:link,
a:active {
  color: #fff;
}

a:visited{
  color:inherit;
}

a:hover{
  text-decoration: underline;
}
</style>
