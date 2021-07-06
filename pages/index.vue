<template>
<div>
    <Nav />
    <Hero />
    <LargeCardDisplay
    :largeCardInfos="largeCardInfos"
    /> 
    <SmallCardDisplay
    :smallCardInfos="smallCardInfos" />
</div>

</template>

<script>
// imported components
import Hero from '../components/Hero.vue'
import LargeCardDisplay from '../components/LargeCardDisplay'
import SmallCardDisplay from '../components/SmallCardDisplay.vue'
import Nav from '../components/Nav.vue'

// imported data
import {largeCardSections} from '../assets/data.js'
import {smallCardSections} from '../assets/data.js'


export default {
    data() {
        return {
            largeCardInfos: largeCardSections,
            smallCardInfos: smallCardSections
        }
    }
}
</script>
