<template>
    <article>
        <img :src="posterSeries" alt="">
        <p>{{ titleSeries }}</p>
    </article>
</template>
<script>
export default {
    name: "SeriesElement",
    props: [
        "posterSeries", "titleSeries"
    ]
}
</script>
<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

article {
    width: calc(100% / 6);
    height: 10rem;
    margin-bottom: 3.5rem;

    img {
        height: 9.2rem;
        width: 8.6rem;
        margin-bottom: 0.5rem;
    }

    p {
        text-transform: uppercase;
        font-size: 0.7rem;
        color: $white;
    }
}
</style>