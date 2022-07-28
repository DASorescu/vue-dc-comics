<template>
    <header>
        <div class="container wrapper">
            <img src="../assets/img/dc-logo.png" alt="DC">
            <nav>
                <ul>
                    <li v-for="(object, index) in this.navmenu" :key="index"><a :href="object.url">{{ object.text }}</a>
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
    height: 15%;
    background-color: #fff;
    padding: 1rem;

    img {
        padding: 1rem;
        max-height: 100%;
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
    width: 60%;

    ul {
        display: flex;
        list-style-type: none;

        li {
            padding: 0.5rem;
            font-size: 10px;
        }
    }
}
</style>