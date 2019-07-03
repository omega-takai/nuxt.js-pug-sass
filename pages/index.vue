<template lang="pug">
  section.container
    div
      logo
      h1.title nuxt.js-v2.8-pug-sass
      h2.subtitle my play ground
      .links
        p Nuxt.js Links
        a.button--green(href="https://ja.nuxtjs.org/" target="_blank")
          | Documentation
        a.button--grey(href="https://github.com/nuxt/nuxt.js" target="_blank")
          | GitHub
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
  min-height: 100vh
  display: flex
  justify-content: center
  align-items: center
  text-align: center
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
.links
  padding-top: 15px
  p
    width: 100%
    font-size: 1.6rem
@mixin button($color: #3b8070)
  display: inline-block
  margin: .5rem 1rem
  border-radius: .4rem
  border: 1px solid $color
  color: $color
  text-decoration: none
  padding: 1rem 3rem
  font-size: 1.6rem
  &:hover
    color: #fff
    background-color: $color
.button--green
  @include button
.button--grey
  @include button(#35495e)
</style>
