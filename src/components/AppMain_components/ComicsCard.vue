<script>
export default {
    props: {
        coverImage: String,
        price: String,
        comicSeries: String,
        category: String
    }
}
</script>

<template>
    <article class="card">
        <div class="img">
            <img :src="coverImage" :alt="comicSeries">
        </div>
        <div class="text">
            <h3>{{ comicSeries }}</h3>
        </div>
    </article>
</template>

<style lang="scss">
.card {
    width: calc(100% / 6 - 20px);
    margin: 0 20px 30px 0;

    .img,
    .text {
        width: 100%;
        margin-bottom: 10px;
    }

    .img {
        height: 220px;
        overflow: hidden;

        img {
            width: 100%;
        }
    }

    .text {
        height: 50px;
        text-transform: uppercase;
    }
}
</style>