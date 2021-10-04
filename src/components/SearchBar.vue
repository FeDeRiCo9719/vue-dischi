<template>

    <form action="">
        <button type="submit">
            <i class="fas fa-search"></i>
        </button>
        <input type="text" placeholder="Search.." name="search">
    </form>

</template>

<script>
export default {
  name: 'SearchBar',
  props: []
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
    .container {
        form {

            input {
               padding: 5px;
               border: none;
               border: 4px solid lightslategray;
               border-radius: 0 5px 5px 0;
               background-color: white;
               outline: none;
            }

            button {
               padding: 5px;
               border: 4px solid lightslategray;
               background-color: lightslategray;
               cursor: pointer;
               border-radius: 5px 0 0 5px;

               i {
                   color: white;
               }
            }
        }
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