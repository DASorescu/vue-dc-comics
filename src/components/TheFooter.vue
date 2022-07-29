<template>
    <footer>
        <div class="top-footer">
            <div class="container">
                <div class="footer-list">
                    <div class="column">
                        <h3>DC Comics</h3>
                        <ul>
                            <li v-for="link in ComicsLinks" :key="link.text">
                                <a :href="link.url" :class="{ active: link.current }">
                                    {{ link.text }}</a>
                            </li>
                        </ul>
                        <h3>Shop</h3>
                        <ul>
                            <li v-for="link in ShopLinks" :key="link.text">
                                <a href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>

                    <div class="column">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="link in Links" :key="link.text">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="column">
                        <h3>Sites</h3>
                        <ul>
                            <li v-for="link in SitesLinks" :key="link.text">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="footer-logo">

                </div>
            </div>
        </div>

        <div class="container">
            <div class="boottom-footer"></div>
        </div>
    </footer>
</template>
<script>
export default {
    name: 'TheFooter',
    props: {
        ComicsLinks: Array,
        Links: Array,
        SitesLinks: Array,
        ShopLinks: Array
    }
}
</script>

<style lang="scss" scoped>
.top-footer {
    height: 260px;
    color: #fff;
    background-image: url(../assets/img/footer-bg.jpg);

    .container {
        height: 100%;
        display: flex;
        justify-content: space-between;
    }

    .footer-logo {
        height: 100%;
        flex-basis: 40%;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-size: cover;
        background-position: center;

    }

    .footer-list {
        flex-basis: 40%;
        display: flex;
        flex-wrap: wrap;

        .column {
            flex-basis: calc(100% / 3);

            li {
                font-size: 10px;
            }

            h3 {
                font-size: 15px;
            }
        }
    }

    a {
        text-decoration: none;
        color: #414141;
    }

    ul {
        padding: 0%;
    }
}
</style>








