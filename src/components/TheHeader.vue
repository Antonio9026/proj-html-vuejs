<script >
export default {
    name: "TheHeader",
    data() {
        return {
            links: [
                {
                    text: "Home"
                }, {
                    text: "About Us"
                }, {
                    text: "Portfolio"
                }, {
                    text: "Our Process"
                }, {
                    text: "Pricing"
                }, {
                    text: "Blog"
                }, {
                    text: "Contact"
                },
            ]
        }
    },

}
</script>

<template>
    <header>
        <div class="header_container">
            <div class="wrapper">
                <div class="logo_container">
                    <img src="../assets/img/logo.png" alt="">
                </div>


                <div class="nav_container">
                    <ul class="nav_list">
                        <li v-for="link in links">
                            <a href="">{{ link.text }}</a>
                        </li>
                    </ul>

                    <div class="button_container">
                        <button>Get a Quote</button>
                    </div>
                </div>
            </div>

        </div>
        <div class="jumbotron">

        </div>

    </header>
</template>

<style lang="scss" scoped>
header {
    display: flex;
    justify-content: center;
    width: 100%;
    position: absolute;
    z-index: 20;
}


.header_container {
    min-width:  94.5%;;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 95px;
    //   background-color: #260262;

}




.wrapper {
    height: 50px;
    min-width: 85.5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav_container {
    display: flex;
    align-items: center;
}

.nav_list {
    display: flex;
    list-style-type: none;
    gap: 23px;
}

a {
    font-size: 18px;
    color: white;
    text-decoration: none;
}

a:hover {
    color: #ff7a1f;
}

button {
    width: 170px;
    height: 51px;
    margin-left: 25px;
    font-size: 18px;
    border-radius: 50px;
    border: none;
    background-color: #FFDFED;
    box-shadow: 5px 5px 10px #888888;
    font-family: 'Chakra Petch', sans-serif;
    ;
}

button:hover {
    background-color: #260262;
    box-shadow: 5px 5px 10px #888888;
    border: 1px solid white;
    color: white;
}</style>