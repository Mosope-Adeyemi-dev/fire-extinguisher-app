<template>
<div class="card">
    <span 
    v-for="card in cards"
    :key="card.id">
        <img :src="require(`@/assets/images/${card.image || 'fel.jpg'}`)" alt="" class="image">
        <h3 class="header">{{card.title}}</h3>
        <p class="snippet">
            {{card.snippet}}
        </p>
    </span>
</div>
</template>

<script>
    export default {
       props: {
           cards: Array
       } 
    }
</script>

<style  scoped>
.card {
        height: 20rem;
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
        flex-direction: row;
        margin-bottom: 40px;
    }
    .image {
        height: 65%;
        border-radius: 0.5rem;
        width: 100%;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
    }
    .snippet {
        color: grey
    }
   span{
       width: 60%;
       margin: 0 20px;
       text-align: justify;
   }
</style>