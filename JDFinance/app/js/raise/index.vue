<template lang="html">
  <div>
    <Header />
    <RSlider />
    <Daily />
    <In />
    <More />
    <Footor cname="mfooter"/>
    <Navbar />
  </div>
</template>

<script>
import Header from '../../js/public/header.vue'
import RSlider from './rslider.vue'
import Footor from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
import Daily from './daily.vue'
import In from "./in.vue"
import More from "./more.vue"
export default {
  components: { Header, RSlider, Footor, Navbar, Daily, In, More }
}
</script>

<style lang="scss">
  .mfooter{
    margin-top: 0!important;
    ul{
      li:first-child{
        display: none;
      }
    }
  }
</style>