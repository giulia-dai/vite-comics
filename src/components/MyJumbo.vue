<script>
export default {
    name: "MyJumbo",

    data() {
        return {
            jumbo: "jumbotron.jpg"
        }
    },
    methods: {
        getImagePath(imagePath) {
            return new URL(imagePath, import.meta.url).href;
        }
    },
}
</script>

<template>
    <div class="wrap">
        <img :src="getImagePath(`../img/${jumbo}`)" class="jumbo">
    </div>
</template>

<style>
.wrap {
    height: 300px;
    width: 100%;
}

.jumbo {
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: top;
}
</style>