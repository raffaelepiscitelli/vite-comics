<template>
    <main>
        <span>Current series</span>
        <listSeries />
        <button>Load more</button>
    </main>
</template>
<script>
import ListSeries from './ListSeries.vue';

export default {
    components: {
        ListSeries
    }
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;


main {
    background-color: $darkgray;
    @include flex (column, center, center);
    position: relative;

    span {
        background-color: $blue;
        border: none;
        color: $white;
        text-transform: uppercase;
        font-weight: bolder;
        font-size: 1.2rem;
        padding: 0.5rem 1.2rem;
        margin-bottom: 1rem;
        position: absolute;
        bottom: 30.5rem;
        left: 17rem;
    }

    button {
        background-color: $blue;
        border: none;
        color: $white;
        text-transform: uppercase;
        font-weight: bolder;
        font-size: 0.6rem;
        padding: 0.5rem 2.5rem;
        margin-bottom: 1rem;
    }
}
</style>