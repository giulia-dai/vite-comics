<script>
export default {
    name: "TheFooter"

}
</script>

<template>
    <footer>
        <!-- footer top -->
        <div class="footer-top">
            <div class="container-footer">
                <div class="container">
                    <ul>
                        <li>
                            <h4>DC COMICS</h4>
                        </li>
                        <li><a href="#">Character</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">Tv</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>

                    <ul>
                        <li>
                            <h4>DC</h4>
                        </li>
                        <li><a href="#">Terms of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscription</a></li>
                        <li><a href="#">Talent Workshop</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>

                    <ul>
                        <li>
                            <h4>SITES</h4>
                        </li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">Dc Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>

                    <ul>
                        <li>
                            <h4>SHOP</h4>
                        </li>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>

            </div>
            <div class="logo-footer">
                <img class="img-footer" src="../img/dc-logo-bg.png" alt="logo dc">
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
                    <div class="social-wrapper">
                        <img src="../img/footer-facebook.png" alt="log facebook">
                        <img src="../img/footer-twitter.png" alt="log twitter">
                        <img src="../img/footer-youtube.png" alt="log youtube">
                        <img src="../img/footer-pinterest.png" alt="log pinterest">
                        <img src="../img/footer-periscope.png" alt="log periscope">
                    </div>

                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
.footer-top {
    margin-top: 3rem;
    background-image: url(../img/footer-bg.jpg);
    background-size: cover;
    padding: 2.5rem;
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
}

li>a:hover {
    color: white;
}

.logo-footer {
    float: right;
    position: relative;
}

.img-footer {
    position: absolute;
    width: 340px;
    top: -300px;
    left: -650px;
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
}

button:hover {
    background-color: #84878B;
    color: black;
}

.follow-container {
    display: flex;
    align-items: center;
    padding: 1rem;
}

.social-wrapper {
    padding: 0 1rem;
}

h3 {
    color: #0585FF;
}

.social-wrapper>img {
    padding: 10px;
    cursor: pointer;
}
</style>