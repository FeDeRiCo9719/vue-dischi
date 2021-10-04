<template>
    <header>
        <div class="container" >
            <div class="logoBox">
                <img src="@/assets/img/spotify-logo.png" alt="LogoImg">
            </div>
            <SearchBar/>
        </div>
    </header>
</template>

<script>
import SearchBar from './SearchBar.vue'

export default {
  name: 'Header',
  components: {
    SearchBar
  },
  props: []
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
    height: 80px;
    width: 100%;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 98%;
        // background-color: blue;
        margin: auto;
    }

    .logoBox {
        height: 80px;
        padding: 15px 0px;
        // background-color: blanchedalmond;

        img {
            height: 100%;
        }
    }

}
</style>