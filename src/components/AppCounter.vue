<script>
export default {
    data() {
        return {
            counters: [
                {

                    title: "700+",
                    text: "Projects done "
                }, {

                    title: "250+",
                    text: "Happy clients"
                }, {

                    title: "25+ ",
                    text: "Team members"
                },
                {

                    title: "12+",
                    text: "Years on the market"
                },
            ]
        }
    },


}
</script>

<template>
    <div class="counter-container">
        <div class="img-top">
            <img src="../assets/img/shape-top.png" alt="">
        </div>
        <div class="title-container">
            <h1>Anidio Quick Facts </h1>
        </div>

        <div class="counter">
            <div class="counter-cards" v-for="counter in counters">
                <div class="title">
                    <h2>{{ counter.title }}</h2>
                </div>
                <div class="text">
                    <h2>{{ counter.text }}</h2>
                </div>
            </div>

        </div>
        <div class="planet-container">
            <img class="planet-img" src="../assets/img/globe.png" alt="">
        </div>
        <div class="img-bottom">
            <img src="../assets/img/shape-bottom.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.counter-container {
    margin-top: 130px;
    min-height: 500px;
    background-image: url(../assets/img/counter-bg.png);
    background-size: cover;
   
    position: relative;
    margin-bottom: 100px;
}

.title-container {
    // max-width: 550px;
    // margin: 0 auto;
    // background-color: #311852;
    position: relative;
    z-index: 40;
}

h1 {

    margin: 40px 0;
    text-align: center;
    font-size: 60px;
    color: white;

}

.counter {
    max-width: 75%;
    min-height: 260px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    padding: 20px 0;
}

.counter-cards {
    width: calc(100%/4);
    width: 220px;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 220px;
    border: 1px solid white;
    border-radius: 40px;

}

.title {
    font-size: 40px;
    color: white;
    z-index: 30;
}
.text{
    font-size: 12px;
    color: #ff7a1f;
    z-index: 30;
}
.planet-container {
    max-width: 500px;
    height: 500px;
    position: absolute;
    z-index: 3;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    // object-fit: contain;

}

.planet-img {
    width: 100%;
    height: 100%;
}

.img-top img {
    z-index: 81;
    position: relative;
    object-fit: contain;
}

.img-bottom {
    height: 45px;
    position: absolute;
    z-index: 25;

}

.img-bottom img {
    height: 100%;
    vertical-align: middle;
}
</style>