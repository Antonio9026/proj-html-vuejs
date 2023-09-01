<script >
import AppHero from "./AppHero.vue"

export default {
    components: {
        AppHero,
    },
    data() {
        return {
            cards: [
                {
                    img: "src/assets/img/smart1.png",
                    title: "3D modeling",
                    text: "We constantly ask questions. It helps us shape your story and deliver the results you crave. Yep, we'll drill deep to deliver above and beyond your expectations. "
                }, {
                    img: "src/assets/img/smart2.png",
                    title: "Collaboration",
                    text: "We constantly ask questions. It helps us shape your story and deliver the results you crave. Yep, we'll drill deep to deliver above and beyond your expectations"
                }, {
                    img: "src/assets/img/smart3.png",
                    title: "Creativity",
                    text: "We constantly ask questions. It helps us shape your story and deliver the results you crave. Yep, we'll drill deep to deliver above and beyond your expectations"
                },
            ]
        }
    },

}
</script>

<template>
    <AppHero></AppHero>
    <section class="smart">
        <div class="smart-img-left">
            <img src="../assets/img/smart.png" alt="">
        </div>
        <div class="smart-cards-container">
            <div class="jumbo-container">
                <h2>Our Love For Animation </h2>
                <h1>We're Storytelling </h1>
                <h1>Experts With Creative</h1>
                <h1>Smarts </h1>
                <p>Our culture inspires the creative and innovative spirit found throughout our Studio. We breathe life into
                    new ideas! </p>
                <div class="cards-container">
                    <div class="card-wrapper" v-for="card in cards">
                        <div class="img-card">
                            <img :src="card.img" alt="">
                        </div>
                        <div class="card">
                            <h3>{{ card.title }}</h3>
                            <p>{{ card.text }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.smart {
    display: flex;
    margin-top: 380px;


}

.smart-img-left {
    width: 500px;
    position: absolute;

}

.smart-img-left img {
    width: 100%;
}

.jumbo-container {
    max-width: 720px;
    margin: 0 auto;
    text-align: center;
    margin-top: 80px;
    margin-left: 400px;
    position: relative;
    z-index: 1;

}

h1 {
    font-size: 55px;
    color: #311852;
}

h2 {
    margin-bottom: 20px;
    color: #4d36dc;
}

p {

    text-align: center;
    font-size: 18px;
    color: #311852;
    font-family: 'Chakra Petch', sans-serif;
}

.cards-container {
    min-width: 1200px;
    display: flex;
    flex-wrap: wrap;
    gap: 25px;
    margin-top: 80px;
 

}

.card-wrapper {
    max-width: 250px;
   width: calc(100%/3);
    border: 1px solid #b2b5d2;
    border-radius: 40px;
}
.card-wrapper:hover{
    border: none;
   
}

.card {
    
    // margin: 0 auto;
    line-height: 30px;
    font-family: "Barlow", sans-serif;
    margin-bottom: 40px;
}

.card h3 {
    font-size: 30px;
    margin: 20px 0;
}
.img-card{
    margin-top: 40px;
}
</style>