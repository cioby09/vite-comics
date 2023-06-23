<script>
export default {
    name: "AppCard",
    props: {
        thumb: String,
        series: String,

    }
}
</script>

<template>
    <div class="card">
        <img :src="thumb" alt="">
        <h4>{{ series }}</h4>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: calc(100% / 6 - 20px);
    margin: 10px;


    img {
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: top;
    }

    h4 {
        color: white;
        margin-top: 5px;
        text-transform: uppercase;
        font-size: 0.6rem;
        font-weight: 300;
    }

}
</style>