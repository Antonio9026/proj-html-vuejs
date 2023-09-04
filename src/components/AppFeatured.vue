<script>

export default {



}
</script>

<template>
    <section class="featured">
        <div class="container">
            <div class="jumbo-wrapper">
                <div class="jumbo-featured">
                    <h4>Our Works </h4>
                    <h1>Featured Productions </h1>
                    <p>Here's just a small sample of some of those projects that we're quite proud of. If you're looking for
                        something specific feel free to get in contact with us. </p>
                </div>
            </div>
            <div class="images-container">
                <div class="first-img">
                    <img src="../assets/img/work1.png" alt="">
                </div>
                <div class="first-img">
                    <img src="../assets/img/work2.png" alt="">
                </div>
                <div class="first-img">
                    <img src="../assets/img/work3.png" alt="">
                </div>
                <div class="first-img">
                    <img src="../assets/img/work4.png" alt="">
                </div>


            </div>
            <div class="button">
                <button>See Our Work</button>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.container {
    // display: flex;
    // justify-content: center;
    margin-top: 130px;
}

.jumbo-wrapper {
    display: flex;
    justify-content: center;
}

.jumbo-featured {
    max-width: 660px;
    text-align: center;
}

h4 {
    font-size: 25px;
    color: #4c36db;
}

h1 {
    font-size: 55px;
    color: #311852;
}

p {
    font-size: 18px;
    color: #311852;
}

.images-container {
    width: 85%;
    margin: 0 auto;
    margin-top: 60px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.first-img {
    width: calc(100%/2);
    width: 550px;
}

img {
    width: 100%;
}
.button{
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top: 40px;
}
button{
    width: 200px;
    height: 50px;
    font-size: 18px;
    border-radius: 100px;
    border: 1px solid #ffdfed;
    background-color: white;
    color: #311852;
    font-family: 'Chakra Petch', sans-serif;
}
</style>