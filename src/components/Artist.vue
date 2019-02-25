<template lang="pug">
  li
    h2: a(:href="artist.url" target="_blank") {{ artist.name }}
    img(:src="artist.image[2]['#text']" :alt="artist.name")
</template>

<script>
  export default {
    name: 'artist',
    props: ['artist']
  }
</script>

<style lang="stylus" scoped>
  ul
    display flex
    flex-direction row
    flex-wrap wrap
  li
    display block
    margin 10px 0
</style>