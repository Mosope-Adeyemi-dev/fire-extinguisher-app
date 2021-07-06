<template>
<div class="whole">
   <div class="hero container">
       <div class="text-container">
            <h1 class="header">Find your fire extinguisher</h1>
            <p class="snippet">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid molestiae consectetur nesciunt odio, id nisi pariatur culpa? Nisi, soluta reprehenderit!</p>
            <button class="button btn">Start looking</button>
       </div>
        <img src="~assets/svg/fire-extinguisher.svg" alt="" class="image">
   </div>
   </div>
</template>

<script>
    export default {
        
    }
</script>

<style  scoped>
.whole{
    position: relative;
}
    .Hero {
        height: 50vh;
        position: relative;
        display: flex;
        padding: 5rem 0;
        align-items: flex-start;
        justify-content: space-between;
    }
    .text-container {
        width: 40%;
        margin-top: 4rem;
        position: absolute;
    }
    .header {
        font-weight: 900;
        font-size: 5rem;
    }
    .snippet {
        color: grey;
        font-size: 1.25rem;
        width: 70%;
    }
    .image {
        width: 27rem;
        margin-top: 4rem;
        float: right;
    }
    .overlay {
        background: rgba(0, 0, 0, 0);
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
    }
    .button {
        padding: 1rem 4rem;
        border-radius: 100rem;
        background-color: rgb(231, 81, 43);
        color: white;
        width: 20rem;
        font-weight: 700;
        transition: 0.5s;
    }
    .button:hover {
        width: 21.5rem;
    }
    @media (max-width: 500px) {
        .Hero {
            height: 40vh;
        }
    }
</style>