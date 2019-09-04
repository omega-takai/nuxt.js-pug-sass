<template lang="pug">
div.wrapper
  header.header
    .links
      p Nuxt.js Links
      a.button--green(href="https://ja.nuxtjs.org/" target="_blank")
        | Documentation
      a.button--grey(href="https://github.com/nuxt/nuxt.js" target="_blank")
        | GitHub

  nuxt.main

  footer.footer
    .links
      p This Project Links
      a.button--grey(href="https://github.com/t--takai/nuxt.js-pug-sass" target="_blank")
        | GitHub
</template>

<style lang="sass" scoped>
.wrapper
  display: grid
  grid-template: 'header' 'main' 'footer' / 1fr
  width: 100vw
  min-height: 100vh
  overflow: hidden

.header
  grid-area: header

.main
  grid-area: main

.footer
  grid-area: footer
</style>
