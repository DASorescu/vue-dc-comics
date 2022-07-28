<template>
    <main>
        <!-- content section -->
        <section class="content-section">
            <div class="container">
                <div class="content">
                    --Content Goes Here--

                </div>

            </div>
        </section>
        <section class="banner ">
            <div class="container">
                <ul>
                    <li><img src="../assets/img/buy-comics-digital-comics.png" alt="buy">
                        <p>DIGITAL COMICS</p>
                    </li>
                    <li><img src="../assets/img/buy-comics-merchandise.png" alt="buy">
                        <p>DC MERCHANDISE</p>
                    </li>
                    <li><img src="../assets/img/buy-comics-subscriptions.png" alt="buy">
                        <p>SUBSCRIPTION</p>
                    </li>
                    <li><img src="../assets/img/buy-comics-shop-locator.png" alt="buy">
                        <p>COMIC SHOP LOCATOR</p>
                    </li>
                    <li><img src="../assets/img/buy-dc-power-visa.svg" alt="buy">
                        <p>DC POWER VISA </p>
                    </li>
                </ul>

            </div>
        </section>
    </main>
</template>

<script>
export default {
    name: 'TheMain',
    data() {
        return {
            assets: [
                {

                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
main {
    height: 30%;
}

.container {
    height: 100%;
}

.content-section {
    background-color: #000;
    height: 50%;
}

.content {
    height: 100%;
    color: #fff;
    display: flex;
    align-items: center;

    font-size: 30px;
}

.banner {
    background-color: #0082F9;
    color: #fff;
    height: 50%;

    .container {
        height: 100%;
    }
}

ul {
    height: 100%;
    display: flex;


    li {
        padding: 2rem;
        flex-basis: 20%;
        display: flex;
        align-items: center;

        img {
            height: 35px;

        }

        p {
            font-size: 10px;
            padding-left: 10px;

        }
    }
}
</style>