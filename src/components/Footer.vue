<template>
    <footer>
        <section class="footer-top">
            <div class="container">
                <div class="footer-menu">
                    <div class="menu-item">
                        <h2>DC comics</h2>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                            <h2>SHOP</h2>
                            <ul>
                                <li>
                                    <a href="#">Shop DC</a>
                                </li>
                                <li>
                                    <a href="#">Shop DC Collectibles</a>
                                </li>
                            </ul>
                        </ul>
                    </div>
                    <div class="menu-item">
                        <h2>DC</h2>
                        <ul>
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy Policy (New)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact Us</a>
                            </li>
                        </ul>
                    </div>
                    <div class="menu-item">
                        <h2>SITES</h2>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png">
                </div>
            </div>
        </section>
        <section class="footer-bot">
            <div class="container">
                <div class="sign-up">
                    <a href="#">SIGN-UP NOW!</a>
                </div>
                <div class="social-link">
                    <ul>
                        <li>
                            <a href="#">Follow Us</a>
                        </li>
                        <li>
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </li>
                    </ul>
                </div>
            </div>  
        </section>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {

        }
    }
}
</script>

<style scoped lang="scss">
    @import "../assets/scss/parzials/_variables";

    .footer-top {
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: repeat-x;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            .footer-menu {
                display: flex;
                flex-wrap: wrap;
                .menu-item {
                    margin-right: 2em;
                    h2{
                        color: white;
                        font-size: 1.5em;
                        text-transform: uppercase;
                        margin-top:  2em;
                    }
                    ul {
                        list-style: none;
                        li a {
                            text-decoration: none;
                            color: grey;
                            line-height: 2em;
                        }
                    }
                }
            }
            .logo {
                text-align: right;
                img {
                    width: 80%;
                    padding-top: 1em;
                }
            }
        }
    }
    .footer-bot {
        background-color: #303030;
        padding: 2em 0;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            .sign-up {
                width: 50%;
                a {
                    padding: 0.8em;
                    border: 2px solid $brand-font-color;
                    text-decoration: none;
                    color: white;
                }
            }
            .social-link {
                width: 50%;
                ul {
                    list-style: none;
                    display: flex;
                    justify-content: flex-end;
                    align-items: center;
                    gap: 2em;
                    a {
                        text-decoration: none;
                        text-transform: uppercase;
                        font-size: 1.5em;
                        color: $brand-font-color;
                    }
                }
            }
        }
    }
</style>