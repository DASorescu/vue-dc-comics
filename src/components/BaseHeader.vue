<template>
    <header>
        <div class="container wrapper">
            <img src="../assets/img/dc-logo.png" alt="DC">
            <nav>
                <ul>
                    <li v-for="(object, index) in this.navmenu" :key="index"><a :href="object.url"
                            :class="{ active: object.current }">{{ object.text }}</a>
                    </li>
                </ul>
            </nav>

        </div>
    </header>
</template>

<script>
export default {
    name: 'BaseHeader',
    data() {
        return {
            navmenu: [

                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
header {

    height: 10%;
    background-color: #fff;


    img {
        padding: 1rem;
        height: 50px;
        width: auto;
    }

    .wrapper {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;

    }
}

nav {
    height: 100%;
    width: 60%;

    ul {
        height: 100%;
        display: flex;
        justify-content: space-between;
        list-style-type: none;
        margin: 0%;

        li {
            padding: 0.5rem;
            font-size: 10px;
        }
    }

    .active {
        border-bottom: 2px solid #0082F9;
    }
}
</style>