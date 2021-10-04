<template>
  <div id="app">    
    <Header @choice="print"/>
    <!-- <Header/> -->
    <Albums/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Albums from './components/Albums.vue'

export default {
  name: 'App',
  components: {
    Header,
    Albums
  },
  methods: {
    print(text) {
      console.log(text);
    }
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss'
</style>
