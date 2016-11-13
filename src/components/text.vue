<template>
  <div :class="$style.text">
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
  }
}
</script>

<style lang="sass" module>

.text{
  font-size:15px;
  composes: yellow from "sass!../common/color.scss";
}

</style>