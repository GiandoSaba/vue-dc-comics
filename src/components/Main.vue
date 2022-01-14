<template>
    <main>
        <section class="content-section">
            <div class="container">
                <h1>--> Content goes here </h1>
            </div>
        </section>
        <section class="card-section">
            <div class="container">
                <ul>
                    <li>
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital-Comics">
                        <a href="#">Digital Comics</a>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-merchandise.png" alt="Digital-Comics">
                        <a href="#">DC Merchandise</a>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="Digital-Comics">
                        <a href="#">Subscriptions</a>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="Digital-Comics">
                        <a href="#">Comic Shop Locator</a>
                    </li>
                    <li>
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="Digital-Comics">
                        <a href="#">DC Power Visa</a>
                    </li>

                </ul>
            </div>
        </section>
    </main>
</template>

<script>
export default {
    name: 'Main',
    data() {
        return {

        }
    }
}
</script>

<style scoped lang="scss">
    @import "../assets/scss/parzials/_variables";
    
    .container {
        color: white;
    }
    .content-section {
        background-color: black;
        .container {
            padding: 3em;
            h1 {
                font-size: 1.5em;
            }
        }
    }
    .card-section {
        background-color: $brand-font-color;
        padding: 2.5em;
        ul {
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 8px;
            li {
                flex-basis: calc(100% / 5);
                display: flex;
                align-items: center;
                justify-content: center;
                img {
                    height: 50px;
                    margin-right: 1em;
                }
                a {
                    text-transform: uppercase;
                }
            }

        }

    }
</style>