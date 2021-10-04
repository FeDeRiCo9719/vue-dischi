<template>
  <section class="AlbumSection">
    <div class="container">
      <div class="boxAlbum" v-for="(item, index) in songs.response" :key="index">
        <Album :info="item" />
      </div>
    </div>
  </section>
</template>

<script>
import axios from 'axios';
import Album from './Album.vue';

export default {
  name: 'Albums',
    components: {
    Album
  },

  data() {
    return {
      songs: {}
    }
  },

  created() {
    axios
    .get('https://flynn.boolean.careers/exercises/api/array/music')
    .then( (res) => {
      this.songs = res.data;
    }); 
  },
  props: []
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  section {
    height: calc(100vh - 80px);
    // padding: 0px 400px;
    display: flex;
    justify-content: center;
    align-items: center;

    .container {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 30px;
      text-align: center;
      width: 60%;

      .boxAlbum {
        background-color: #2E3A46;
        width: 180px;
        height: 350px;
        padding: 20px;
      }
    }        
  }

</style>