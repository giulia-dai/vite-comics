<script>
export default {
    name: "TheFooter",
    data() {
        return {
            DC_COMICS: [
                "Character",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            SHOPS: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            DC: [
                "Terme of Use",
                "Privacy Policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPCS Certificates",
                "Ratings",
                "Shop Help",
                "Contact us"
            ],
            SITES: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ],
            SOCIALS: [
                "footer-facebook.png",
                "footer-twitter.png",
                "footer-youtube.png",
                "footer-pinterest.png",
                "footer-periscope.png"
            ]
        }
    },
    methods: {
        getImagePath(imagePath) {
            return new URL(imagePath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <footer>
        <!-- footer top -->
        <div class="footer-top">
            <div class="container-footer">
                <div class="container">

                    <div>
                        <h4>DC COMICS</h4>

                        <ul>
                            <li v-for="comic in DC_COMICS"><a href="#">{{ comic }}</a></li>
                        </ul>
                    </div>

                    <div>
                        <h4>SHOP</h4>
                        <ul>
                            <li v-for="shop in SHOPS"><a href="#">{{ shop }}</a></li>
                        </ul>
                    </div>

                    <div>
                        <h4>DC</h4>

                        <ul>
                            <li v-for="link_DC in DC"><a href="#">{{ link_DC }}</a></li>
                        </ul>
                    </div>

                    <div>
                        <h4>SITES</h4>

                        <ul>
                            <li v-for="site in SITES"><a href="#">{{ site }}</a></li>
                        </ul>
                    </div>
                </div>
                <div class="logo-footer">
                    <img class="img-footer" src="../img/dc-logo-bg.png" alt="logo dc">
                </div>
            </div>
        </div>
        <!-- footer bottom -->

        <div class="footer-bottom">
            <div class="container-bottom">

                <div class="sign-in">
                    <button>SIGN-UP NOW!</button>
                </div>

                <div class="follow-container">
                    <h3>FOLLOW US</h3>
                    <ul class="social-wrapper">
                        <li v-for="social in SOCIALS">
                            <img :src="getImagePath(`../img/${social}`)">
                        </li>
                    </ul>

                </div>
            </div>
        </div>


    </footer>
</template>

<style lang="scss" scoped>
.footer-top {
    background-image: url(../img/footer-bg.jpg);
    background-size: cover;
    padding: 1.5rem;

}

.container {
    margin: auto;
    margin-top: 1rem;
    max-width: 1170px;
    display: flex;
}

ul {
    list-style: none;
}

h4 {
    color: white;
    padding: 0.5rem;
}

li>a {
    padding: 0.5rem;
    text-decoration: none;
    color: #84878B;

    &:hover {
        color: white;
    }
}

.logo-footer {
    float: right;
    position: relative;
}

.img-footer {
    position: absolute;
    width: 280px;
    top: -280px;
    left: -500px;
}

/* footer boottom */
.footer-bottom {
    background-color: #303030;
}

.container-bottom {
    margin: auto;
    max-width: 1170px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

button {
    padding: 1rem;
    border: 2px solid #0585FF;
    background-color: #303030;
    color: white;

    &:hover {
        background-color: #84878B;
        color: black;
    }
}

.follow-container {
    display: flex;
    align-items: center;
    padding: 1rem;
}

.social-wrapper {
    padding: 0 1rem;
    display: flex;
}

h3 {
    color: #0585FF;
}

.social-wrapper>li {
    padding: 7px;
    cursor: pointer;
}
</style>