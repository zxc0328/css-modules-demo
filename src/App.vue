<template>
  <div :class="$style.app">
    <div :class="$style.text">
      some text
    </div>
    <main-text></main-text>
  </div>
</template>

<script>
import text from "./components/text.vue";

export default {
  created () {
    console.log(this.$style)
  },
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
    'main-text':text
  }
}
</script>

<style lang="sass" module>

.app{
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.text{
  font-size: 20px;
  composes: red from "sass!./common/color.scss";
}


</style>
