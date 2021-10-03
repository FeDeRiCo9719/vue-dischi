<template>
  <section>
    <div class="container">
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
      <div>a</div>
    </div>
    <Album/>
  </section>
</template>

<script>
import Album from './Album.vue'

export default {
  name: 'Albums',
    components: {
    Album
  },
  props: []
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  section {
    height: calc(100vh - 80px);
    padding: 0px 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    .container {
      background-color: rgba(0, 0, 0, 0.479);
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 30px;

      div {
        background-color: rgba(164, 202, 183, 0.479);
        width: 180px;
        height: 300px;
      }

    }
  }

</style>