<script >
export default {
    data() {
        return {
            cards: [
                {
                    image: "src/assets/img/process1.png",
                    title: "Scripting",
                    text: "We'll take your idea and create a tecnical script wich consist of action notes and animation description "
                }, {

                    image: "src/assets/img/process2.png",
                    title: "Pre-Production",
                    text: "We'll take your idea and create a tecnical script wich consist of action notes and animation description  "
                },
            ]
        }
    },

}
</script>

<template>
    <div class="container-img">
        <div class="process-img">
            <img src="../assets/img/process-thumb.png" alt="">
        </div>
    </div>
    <div class="container">

        <div class="process-right">
            <div class="header">
                <h4>Our Process</h4>
                <h1>Our Process for </h1>
                <h1>Your Animation </h1>
                <h1>Production</h1>
                <p>We have an effective process for working on animation </p>
            </div>
            <div class="process-cards">
                <div class="card" v-for="card in cards">
                    
                        <div class="img-card-process">
                            <img :src="card.image" alt="">
                        </div>
                    
                    <div class="content">
                        <h2>{{ card.title }}</h2>
                        <p>{{ card.text }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    display: flex;
    margin-left: 650px;
    margin-top: 140px;
   
}


.header {
    width: 80%;
    margin: 0 auto;
}

h4 {
    font-size: 22px;
    color:#4d36dc;
}

h1 {
    font-size: 55px;
    color: #311852;
}

.header p {
    font-size: 18px;
    color: #311852;
}

.process-cards {
    display: flex;
    gap: 20px;
    margin-top: 50px;
    text-align: center;
   
}

.card {
    max-width: 260px;
    border: 1px solid #b2b5d2;
    border-radius: 50px;
}

.content {
    width: 80%;
    margin: 0 auto;
    line-height: 30px;
    margin-bottom: 40px;
}

.content h2 {
    margin: 20px 0;
}

.container-img {
    width: 900px;
    position: relative;
}
.container-img{
    
}
.process-img {
    position: absolute;
    left: -275px;
    top: 120px;
}

.process-img img {
    width: 100%;
}

.img-card-process {
    width: 130px;
    height: 130px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #fff5f0;
    margin-top: 40px;
    border-radius: 50%;
}

.img-card-process img {
    width: 80px;
    height: 80px;
}
</style>