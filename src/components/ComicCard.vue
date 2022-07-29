<template>
    <div class="card">
        <figure>
            <img :src="image" :alt="title">
        </figure>
        <p>{{ title }}</p>
    </div>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        image: String,
        title: String,
    }

}

</script>
<style lang="scss" scoped>
.card {
    height: 80%;
    width: 100%;
    padding: 0.5rem;

    figure {
        width: 100%;
        margin: 0%;
    }

    img {
        max-width: 100%;
        height: auto;
        display: block;
    }

    p {
        font-size: 15px;
        text-align: start;
    }
}
</style>
