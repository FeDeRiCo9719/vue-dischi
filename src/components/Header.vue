<template>
    <header>
        <div class="container" >
            <div class="logoBox">
                <img src="@/assets/img/spotify-logo.png" alt="LogoImg">
            </div>
            
            <select name="" id=""  v-model="genreSelected" @change="$emit('choice', genreSelected)" >  <!-- @change="SelectGenre" -->
                <option disabled value="">Select a Genre</option>
                <option>Pop</option>
                <option>Jazz</option>
                <option>Metal</option>
                <option>Rock</option>
            </select> 
            <!-- <span>{{genreSelected}}</span> -->
        </div>
    </header>
</template>

<script>

export default {
    name: 'Header',
    data() {
        return {
            genreSelected:'',
        }
    },

    // methods: {
    //     SelectGenre() {
    //         console.log(this.genreSelected);
    //         this.$emit('choice', this.genreSelected )
    //     }
    // }
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

    select {
        padding: 5px ;
        border-radius: 5px;
        outline: none;
    }
}
</style>