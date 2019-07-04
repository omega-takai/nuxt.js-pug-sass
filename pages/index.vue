<template lang="pug">
  section.container
    div
      logo
      h1.title nuxt.js-v2.8-pug-sass
      h2.subtitle my play ground
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="sass" scoped>
.container
  min-height: 50vh
  display: flex
  justify-content: center
  align-items: center
  text-align: center
  flex-wrap: wrap

.title
  display: block
  font-weight: 300
  font-size: 100px
  color: #35495e
  letter-spacing: 1px

.subtitle
  font-weight: 300
  font-size: 42px
  color: #526488
  word-spacing: 5px
  padding-bottom: 15px
</style>
