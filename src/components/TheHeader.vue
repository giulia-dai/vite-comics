<script>
export default {
    name: "TheHeader",
    data() {
        return {
            logo: "dc-logo.png",

            sections: [
                {
                    text: "CHARACTERS"
                },
                {
                    text: "COMICS"
                },
                {
                    text: "MOVIES"
                },
                {
                    text: "TV"
                },
                {
                    text: "GAMES"
                },
                {
                    text: "COLLECTIBLES"
                },
                {
                    text: "VIDEOS"
                },
                {
                    text: "FANS"
                },
                {
                    text: "NEWS"
                },
                {
                    text: "SHOP"
                }
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
    <header>
        <nav>
            <div class="nav-container">
                <div class="logo-wrapper">
                    <img class="logo" :src="getImagePath(`../img/${logo}`)">
                </div>

                <ul>
                    <li v-for="section in sections"><a href="#" class="size">{{ section.text }}</a></li>

                </ul>
            </div>

        </nav>
    </header>
</template>

<style lang="scss" scoped>
nav {
    margin: auto;
    margin-top: 1rem;
    max-width: 1170px;
}

.nav-container {
    display: flex;
    justify-content: space-between;
}

.logo-wrapper {
    padding: 1rem;
}

ul {
    display: flex;
    align-items: center;
    list-style: none;
}

li>a {
    padding: 0.6rem;
    text-decoration: none;
    color: black;
    font-size: 14px;

    &:hover {
        color: #008FFA;
    }
}
</style>