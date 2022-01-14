<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png">
            </div>
            <div class="header-menu">
                <ul>
                    <li>
                        <a href="#">Character</a>
                    </li>
                    <li class="active">
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">Tv</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Collectibles</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">Fans</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                    <li>
                        <a href="#">Shop</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            
        }
    }
}
</script>

<style scoped lang="scss">
    @import "../assets/scss/parzials/_variables";


    .container {
        display: flex;
        align-items: center;
        height: $header-height;
        .logo {
            flex-basis: 30%;
            img {
                width: 70px;
            }
        }
        .header-menu {
            height: 100%;
            ul {
                list-style: none;
                display: flex;
                flex-wrap: nowrap;
                height: 100%;
                li {
                    height: 100%;
                    line-height: $header-height;
                    a {
                        text-transform: uppercase;
                        font-weight: bold;
                        font-size: 0.8em;
                        padding: 1em;
                    }
                    &.active {
                        position: relative;
                        &::after {
                            content: '';
                            width: 100%;
                            height: 3px;
                            background-color: $brand-font-color;
                            position: absolute;
                            top: 98%;
                            left: 0;
                        }
                        a {
                            color: $brand-font-color;
                        }
                    }
    
                }
            }            
        }
    }
</style>