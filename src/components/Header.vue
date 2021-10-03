<template>
    <header>
        <div class="logoBox">
            <img src="@/assets/img/spotify-logo.png" alt="LogoImg">
        </div>
    </header>
</template>

<script>
export default {
  name: 'Header',
  props: []
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
    height: 80px;
    width: 100%;

    .logoBox {
        height: 80px;
        padding: 15px;

        img {
            height: 100%;
        }
    }

}
</style>