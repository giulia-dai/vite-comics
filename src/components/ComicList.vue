<script>
export default {
    name: "ComicList",
    props: {
        thumb: Object,
    }
}
</script>

<template>
    <div class="cards">
        <div class="wrapper">
            <img :src="thumb.thumb">
        </div>
        <h4>{{ thumb.series }}</h4>
    </div>
</template>

<style lang="scss" scoped>
.cards {
    width: calc(100% / 6 - 20px);
    margin: 10px;
    cursor: pointer;

    img {
        width: 100%;
        min-height: 220px;
    }
}
</style>