<template lang="">
    <header>
        <div class="header-container">
            <section class=logo>
                <img src="../assets/imgs/dc-logo.png" alt="">
            </section>
            <section class="navbar">
                <ul>
                    <li>
                        Characters
                    </li>
                    <li>
                        Comics
                    </li>
                    <li>
                        Movies
                    </li>
                    <li>
                        Tv
                    </li>
                    <li>
                        Games
                    </li>
                    <li>
                        Collectibles
                    </li>
                    <li>
                        Videos
                    </li>
                    <li>
                        Fans
                    </li>
                    <li>
                        News
                    </li>
                    <li>
                        Shop
                    </li>
                </ul>
            </section>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader'
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    .header-container {
        @include flex (
            row, space-around, center
        );
        margin: 1rem 6rem 1rem;
        section.logo img {
            height: 4rem;
        };

        ul {
            @include flex (
                row, center, center
            );
            list-style-type: none;
        };

        li {
            padding: 0.8rem;
            font-size: 0.6rem;
            text-transform: uppercase;
            font-weight: bolder;
        };
    }
</style>
