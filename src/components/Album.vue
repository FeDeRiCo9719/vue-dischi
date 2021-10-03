<template>
    
    <div>
        <div class="boxSongImg">
            <img :src="info.poster" alt="info.author">
        </div>
        <h3>{{ info.title }}</h3>
        <h5>{{ info.author }}</h5>
        <h5>{{ info.year }}</h5>
    </div>

</template>

<script>
export default {
    name: 'Album',
    props: {
      info: Object
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    .boxSongImg {
        background-color: cadetblue;
        height: 140px;
        width: 140px;
        margin-bottom: 20px; 
        
        img {
            width: 100%;
        }
    }

    h3 {
        margin-bottom: 20px;
        color: white;
        font-size: 24px;
        font-weight: 500;
    }

    h5 {
        color: grey;
        font-size: 14px;
        font-weight: 400;  
                                
    }

</style>