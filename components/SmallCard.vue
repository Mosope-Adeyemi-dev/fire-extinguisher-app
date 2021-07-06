<template>
    <div class="container">
        <div class="card-container" 
        v-for="card in cards" 
        :key="card.id">
            <img :src="require(`@/assets/images/${card.image}`)" alt="" class="image">
        </div>
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
.container{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-evenly;
    margin-bottom: 40px;
}
.card-container {
        width: 20%;
        height: 12.5rem;
        margin: 0 10px;
        border-radius: 0.5rem;
        overflow: hidden;
        margin-bottom: 1.5rem;
        cursor: pointer;
    }

    .image {
        width: 100%;
        height: 100%
    }
</style>