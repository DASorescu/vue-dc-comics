<template>
  <div id="app">
    <Header />
    <Main />
    <Footer :ComicsLinks="ComicsLinks" :Links="Links" :SitesLinks="Sites" :ShopLinks="Shop" />
  </div>
</template>

<script>

import BaseHeader from './components/BaseHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'

export default {
  name: 'Dc-Comics',
  components: {
    Header: BaseHeader,
    Main: TheMain,
    Footer: TheFooter
  },
  data() {
    return {
      ComicsLinks: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
      Links: [
        {
          text: "Terms of use",
          url: "#",
        },
        {
          text: "Privacy policy(New)",
          url: "#",
          current: true,
        },
        {
          text: "Ad choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      Sites: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD MAgazine",
          url: "#",
          current: true,
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Visa",
          url: "#",
        },
      ],
      Shop: [{ text: "Shop DC" }, { text: "Shop DC Collectibles" }],
    };
  },
}


</script>

<style lang="scss">
@import './assets/scss/style.scss';

#app {
  height: 100%;
  width: 100%;
}
</style>

