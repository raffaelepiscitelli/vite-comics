<template lang="">
    <footer>

        <div class="up-footer-container">

            <div>

                <div>

                    <p>DC Comics</p>

                    <ul class="dc-comics">
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
                            Videos
                        </li>
                        <li>
                            News
                        </li>
                    </ul>

                    <p>Shop</p>

                    <ul>
                        <li>
                            Shop Dc
                        </li>
                        <li>
                            Shop Dc Collectibles
                        </li> 
                    </ul>

                </div>

                <div>

                    <p>DC</p>

                    <ul>
                        <li>
                            Term Of Use
                        </li>
                        <li>
                            Privacy policy (New)
                        </li>
                        <li>
                            Ad Choises
                        </li>
                        <li>
                            Advertising
                        </li>
                        <li>
                            Jobs
                        </li>
                        <li>
                            Subscriptions
                        </li>
                        <li>
                            Talent Workshops
                        </li>
                        <li>
                            CPSC Certificates
                        </li>
                        <li>
                            Ratings
                        </li>
                        <li>
                            Shop Help
                        </li>
                        <li>
                            Contact Us
                        </li>
                    </ul>

                </div>

                <div>

                    <p>Sites</p>

                    <ul>
                        <li>
                            DC
                        </li>
                        <li>
                            MAD Magazine
                        </li>
                        <li>
                            DC Kids
                        </li>
                        <li>
                            DC Universe
                        </li>
                        <li>
                            DC Power Visa
                        </li>
                    </ul>

                </div>      

            </div>

            <div>

                <img src="../assets/imgs/dc-logo-bg.png" alt="">

            </div>

        </div>
        
        <div class="down-footer-container">

            <div>
                <button>Sign-up now!</button>
            </div>

            <div>

                <button>Follow us</button>

                <img src="../assets/imgs/footer-facebook.png" alt="">

                <img src="../assets/imgs/footer-twitter.png" alt="">

                <img src="../assets/imgs/footer-youtube.png" alt="">

                <img src="../assets/imgs/footer-pinterest.png" alt="">

                <img src="../assets/imgs/footer-periscope.png" alt="">

            </div>

        </div>

    </footer>
</template>

<script>
    export default {
        name: 'AppFooter'
    };
    </script>

    <style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    footer {
        background-image: url(../assets/imgs/footer-bg.jpg);
        background-size: cover;

        .up-footer-container {

            @include flex (row, space-between, center);

            padding: 0rem 16rem 0rem;

            div:nth-child(1) {
                @include flex (row, start, start);

                p {
                    color: $white;
                    text-transform: uppercase;
                    font-weight: bolder;
                    font-size: 0.9rem;
                    margin-bottom: 0.8rem;
                };

                ul {
                    list-style-type: none;
                    margin-right: 1rem;
                };

                .dc-comics {
                    margin-bottom: 1rem;
                }

                li {
                    color: $light-gray;
                    padding: 0.1rem;
                    font-size: 0.7rem;
                };

                div:nth-child(1) {
                    @include flex (column, start, start);
                };
            };

            div:nth-child(2) {
                img {
                    height: 25rem;
                    object-fit: none;
                    width: 141%;
                    position: relative;
                    right: 13rem;
                }
            };
        };

        .down-footer-container {
            @include flex (row, space-between, center);
            padding: 1.5rem 16rem 1.5rem;
            background-color: $gray;

            div:nth-child(1) {
                button {
                    background-color: $gray;
                    border: 2px solid $blue;
                    color: $white;
                    text-transform: uppercase;
                    font-weight: bolder;
                    font-size: 0.9rem;
                    padding: 0.5rem;
                }
            };

            div:nth-child(2) {
                @include flex (row, space-around, center);

                img {
                    padding: 0.5rem;
                    height: 2.7rem;
                };

                button {
                    background-color: $gray;
                    border: none;
                    color: $blue;
                    text-transform: uppercase;
                    font-weight: bolder;
                    font-size: 0.9rem;
                    margin-right: 1rem;
                };
            };

        };
    };
</style>