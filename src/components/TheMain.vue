<script>
import AppHero from "./AppHero.vue"
import AppSmartCards from "./AppSmartCards.vue"
import AppCounter from "./AppCounter.vue"
import AppFeatured from "./AppFeatured.vue"
import AppProcess from "./AppProcess.vue"
export default {
    components: {
        AppHero,
        AppSmartCards,
        AppCounter,
        AppFeatured,
        AppProcess,
    },


}
</script>

<template>
    <main>
        <AppHero></AppHero>
        <AppSmartCards></AppSmartCards>
        <AppCounter></AppCounter>
        <AppFeatured></AppFeatured>
        <AppProcess></AppProcess>
    </main>
</template>

<style lang="scss" scoped>

</style>