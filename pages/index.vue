<template>
<header class="header">
  <Transition>
  <div class="show-roadmap" v-if="flag">
      <div class="show-roadmap-wrapper">
        <div class="show-roadmap-exit" @click="flag = false">
          <img src="/img/exit.svg" alt="">
        </div>
        <img src="/img/roadmap.png" alt="">
      </div>
    </div>
  </Transition>
    <nav class="nav container">
      <a ref="/" class="logo">
        <img src="/img/logo.svg" alt="" class="">
        <p class="logo__text">Ayako</p>
      </a>
      <ul class="nav-item">
        <li class="nav-item__link">Community</li>
        <li class="nav-item__link">Market</li>
        <li class="nav-item__link">Trending</li>
      </ul>
      <a href="/" class="nav-account">
        <img src="/img/account.svg" alt="" class="nav-account__img">
        <p class="nav-account__text">My Account</p>
      </a>
    </nav>
    <div class="container flex">
      <div class="row">
        <div class="content-wrapp">
          <div class="content">
            <p class="title">Nft’s that <br>are outta this world</p>
            <p class="text">Ayako is a collection of 2,222 Yōkai powered by $AYKOLSEP </p>
            <div class="images">
              <img src="/img/rate.svg" alt=""><img src="" alt="">
            </div>
          </div>
          <div class="roadmap">
            <button class="roadmap__button"  @click="flag = true">View roadmap</button>
            <img src="/img/hide-roadmap.png" alt="">
          </div>
        </div>

      </div>

      <div class="cards">
        <div class="card-info">
          <div class="card-info-item">
            <p class="card-info-item__text">Mint Price </p>
            <p class="card-info-item__text">1 SOL</p>
          </div>
          <div class="card-info-item">
            <p class="card-info-item__text">Followers</p>
            <p class="card-info-item__text">10.6K</p>
          </div>
          <button class="card__button">
            <a href="https://twitter.com/Ayako_sol">Twitter</a>
          </button>
        </div>
        <img src="/img/cards.png" alt="">
      </div>
    </div>
</header>
</template>

<script>

//import { mapActions, mapGetters, mapState } from 'vuex'

export default {
  name: 'IndexPage',
  layout : 'main_layout',
  data: ()=>({
    flag: true,
  }),
  async mounted() {
    // this.$nextTick(() => {
    //   this.$nuxt.$loading.start()
    //   this.$nuxt.$loading.finish()
    // })


  },
  computed: {
    // ...mapGetters({
    //   flag: 'getItem/CloaseLoadingGet',
    // }),
  },
  methods: {
    // ...mapActions({
    //   flag: 'getItem/CloaseLoadingGet',
    // }),
  }

}
</script>


