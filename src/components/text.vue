<template>
  <div :class="$style.text" v-foo="this.bar">
    text from anonther component
  </div>
</template>

<script>
export default {
  name: 'text',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods:{
    bar() {
      console.log("ddd")
    }
  }
}
</script>

<style lang="sass" module>

.text{
  font-size:15px;
  composes: yellow from "sass!../common/color.scss";
}

</style>