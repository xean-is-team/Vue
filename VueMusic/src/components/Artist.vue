<template lang="pug">
  li.artist
    h2: a(v-bind:href="artist.url" target="_blank") {{artist.name}}
    img(v-bind:src="artist.image[2]['#text']")
</template>

<script>
export default {
  name: 'artist',
  props: ['artist']
}
</script>

<style lang="stylus" scoped>
li.artist
  padding 0px 20px 0px 20px
  display inline-block
  margin 10px 0
h2
  width 174px
</style>
