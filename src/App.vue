<script >
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"
import TheMain from "./components/TheMain.vue"
import MyJumbo from "./components/MyJumbo.vue"




export default {
    components: {
        TheHeader,
        TheMain,
        MyJumbo,
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
        <MyJumbo></MyJumbo>
        <TheMain></TheMain>
    </main>

    <footer>
        <TheFooter></TheFooter>
    </footer>
</template>

<style lang="scss">
@use './styles/general.scss' as *;

html {
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

main {
    background-color: black;
    color: white;
}
</style>
