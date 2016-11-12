<template>
  <div :class="$style.app">
    <div :class="$style.text">
      some text
    </div>
    <div :class="$style.text1">
      some text1
    </div>
  </div>
</template>

<script>
export default {
  created () {
    console.log(this.$style)
  },
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="sass" module>

.app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.red {
  color: red;
}
.text{

  composes: large from "sass!./common/color.scss";
  composes: red from "sass!./common/color.scss";
}

.text1{
  font-size:18px;
  composes: red from "sass!./common/color.scss";
}

</style>
