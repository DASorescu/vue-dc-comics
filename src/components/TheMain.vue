<template>
    <main>
        <TheJumbo />
        <!-- content section -->
        <section class="content-section">
            <button class="current-series">CURENT SERIES</button>
            <div class="container">
                <div class="content">
                    <ul class="comic-cards-section">
                        <li v-for="(object, index) in this.assets" :key="index">
                            <ComicCard :image="object.thumb" :title="object.series" />
                        </li>
                    </ul>
                </div>
                <div class="button-section">
                    <button>LOAD MORE</button>
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
import TheJumbo from './TheJumbo.vue';
import ComicCard from './ComicCard.vue';
export default {
    name: 'TheMain',
    data() {
        return {
            assets: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },
    components: {
        ComicCard,
        TheJumbo,
    }
}
</script>

<style lang="scss" scoped>
.container {
    height: 100%;
}

.content-section {
    background-color: #1C1C1C;
    height: 50%;
    padding: 1rem 2rem;
    position: relative;

    .current-series {
        background-color: #0082F9;
        color: #fff;
        padding: 5px 10px;
        height: 35px;
        width: 150px;
        border-width: 0;
        border-style: none;
        border: 1px solid #0082F9;
        border-image: none;
        position: absolute;
        left: 20%;
        top: -18px;
    }

    .button-section {
        display: flex;
        justify-content: center;

        button {
            background-color: #0082F9;
            color: #fff;
            height: 40px;
            width: 200px;
            border-width: 0;
            border-style: none;
            border-color: #0082F9;
            border-image: none;
        }
    }
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

        ul {
            margin-top: 0%;
            padding-left: 0%;
            justify-content: space-between;
            margin-bottom: 0%;
        }
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

.comic-cards-section {
    height: 100%;
    margin: 0%;
    padding: 0%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;

    li {
        padding: 0;
        flex-basis: 15%;
        height: 100%;
    }
}
</style>
