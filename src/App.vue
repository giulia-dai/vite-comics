<script >
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"


export default {
    components: {
        TheHeader,
        TheFooter
    },
    data() {

    },
    methods: {

    },
}
</script>

<template>
    <header>
        <TheHeader></TheHeader>

    </header>

    <main>
        <h1>-> Main goes here -></h1>
    </main>

    <footer>
        <TheFooter></TheFooter>
    </footer>
</template>

<style>
html {
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

main {
    background-color: black;
    color: white;
}
</style>
