<script>
export default {
    name: "TheHeader"
}
</script>

<template>
    <header>
        <nav>
            <div class="nav-container">
                <div class="logo-wrapper">
                    <img src="../img/dc-logo.png" alt="logo Dc">
                </div>

                <ul>
                    <li><a href="#">CHARACTERS</a></li>
                    <li><a href="#">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </div>

        </nav>
    </header>
</template>

<style scoped>
nav {
    margin: auto;
    margin-top: 1rem;
    max-width: 1170px;
}

.nav-container {
    display: flex;
    justify-content: space-between;
}

ul {
    display: flex;
    align-items: center;
    list-style: none;
}

li>a {
    padding: 1rem;
    text-decoration: none;
    color: black;
}

li>a:hover {
    color: #008FFA;
}
</style>