<template>
   <div class="container">
   <span v-for="cardInfo in largeCardInfos"
   :key="cardInfo.id">

       <h4 class="header">
           {{cardInfo.title}}
       </h4>
       <p class="snippet">
           {{cardInfo.snippet}}
       </p>
       <div class="cards-container">
           <LargeCard 
           :cards="cardInfo.cards" />
        </div>
    </span>
   </div>
</template>

<script>
import LargeCard from "../components/LargeCard.vue"
    export default {
        props: {
            largeCardInfos: Array
        },
    }
</script>

<style scoped>
.container {
    padding-top: 35rem;
}
    .header {
        font-weight: 700;
        font-size: 1.5rem;
    }
    .snippet {
        color: grey;
        margin-bottom: 1.5rem;
    }
    .cards-container {
        display: flex;
        justify-content: space-between;
    }
    
</style>