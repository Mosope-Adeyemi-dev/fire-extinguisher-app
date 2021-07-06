<template>
<div class="container">
    <div 
    v-for="cardInfo in smallCardInfos"
    :key="cardInfo.id">
        <h4 class="header">
            {{cardInfo.title}}
        </h4>
        <div class="card-container">
        <SmallCard :cards="cardInfo.cards"/>
        </div>
    </div>
 </div>
</template>

<script>
    export default {
        props: {
            smallCardInfos: Array
        }
    }
</script>

<style  scoped>
 .container {
        padding: 2rem 0
    }

    .header {
        font-weight: 700;
        font-size: 1.5rem;
        margin-bottom: 0.3rem;
    }

    .card-container {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
</style>