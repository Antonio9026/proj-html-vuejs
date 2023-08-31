<script >

</script>

<template>
    <div class="hero-section">
        <div class="planet-top">
            <img src="../assets/img/globe3.png" alt="" class="planet-top-img">
        </div>
        <div class="planet-left">
            <img src="../assets/img/globe1.png" alt="" class="planet-left-img">
        </div>
        <div class="moon">
            <img src="../assets/img/globe2.png" alt="" class="moon-img">
        </div>
        <div class="spaceship">
            <img src="../assets/img/light.png" alt="" class="spaceship-img">
        </div>

        <div class="container_dots_left">
            <img class="dots-left-img" src="../assets/img/dots-left.png" alt="">
        </div>
        <div class="container_dots_right">
            <img class="dots-right-img" src="../assets/img/dots-right.png" alt="">
        </div>
        <div class="jumbo-container">
            <div class="j-wrapper">
                <div class="container_img_left">
                    <img class="left-img" src="../assets/img/left-man.png" alt="">
                </div>
                <div class="center">
                    <h2>Imagine, Create, Experience</h2>
                    <h1>We Animate</h1>
                    <h1>With Ninja-Like Precision</h1>
                    <p>We are a character-driven animation studio striving to make high-quality animations.</p>
                    <div class="buttons-container">
                        <button class="b-left">Start a Project</button>
                        <button class="b-right">Portfolio</button>
                    </div>
                </div>
                <div class="container-img-right">
                    <img class="right-img" src="../assets/img/right-man.png" alt="">
                </div>
            </div>



        </div>
        <div class="bottom-bg-image">
            <img src="../assets/img/bottom-shape.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.hero-section {
    position: relative;
    padding-top: 160px;
    display: flex;
    background-image: url("../assets/img/banner-bg.png");
    background-position: top;
    min-height: 950px;

    .container_img_left {
        padding-top: 85px;
        max-width: 220px;

        .left-img {

            width: 100%;
        }
    }

    .container-img-right {
        padding-top: 85px;
        margin-left: 15px;
        max-width: 220px;

        .right-img {
            width: 100%;
        }

    }

    .jumbo-container {
        text-align: center;
        z-index: 1;

        // min-height: max-content;
        .j-wrapper {
            width: 100%;
            display: flex;
        }

        h1 {
            font-size: 75px;
            color: white;
        }

        h2 {
            padding-bottom: 20px;
            color: #ff7a1f;
        }

        p {
            padding-top: 10px;
            font-size: 22px;
            color: white;
        }


        .buttons-container {
            display: flex;
            justify-content: center;
            padding-top: 40px;
            gap: 0 20px;

            .b-left {
                width: 190px;
                height: 51px;
                margin-left: 20px;
                font-size: 18px;
                border-radius: 50px;
                border: none;
                background-color: #FFDFED;
                box-shadow: 5px 5px 10px #888888;
                font-family: 'Chakra Petch', sans-serif;

            }

            .b-left:hover {
                background-color: #260262;
                box-shadow: 5px 5px 10px #888888;
                border: 1px solid white;
                color: #FFDFED;
            }

            .b-right {
                width: 140px;
                height: 51px;
                color: #FFDFED;
                background-color: #260262;
                box-shadow: 5px 5px 10px #888888;
                border: 1px solid white;
                border-radius: 50px;
                font-size: 18px;
                font-family: 'Chakra Petch', sans-serif;
            }
        }
    }
}


.planet-left {
    position: absolute;
    width: 130px;
    left: 123px;
    top: 129px;
}

.planet-left-img {
    width: 100%;

}

.moon {
    position: absolute;
    width: 100px;
    left: 864px;
    top: 174px;
}


.moon-img {
    width: 100%;
}

.spaceship {
    position: absolute;
    width: 120px;
    left: 1110px;
    top: 100px;
}

.spaceship-img {

    width: 100%;
}

.planet-top {
    position: absolute;
    width: 285px;
    left: 445px;
    top: -180px;

}

.planet-top-img {

    width: 100%;
}

.container_dots_left {
    position: absolute;
    left: 50px;
    top: 150px;

}

.container_dots_right {
    position: absolute;
    z-index: 0;
    max-width: 750px;
    right: 100px;
    top: 80px;
}

.dots-left-img {
    width: 100%;

}

.bottom-bg-image {
    position: absolute;
    bottom: -40px;
    left: 0;
    width: 100%;
    overflow: hidden;
    height: 200px;

}
</style>
