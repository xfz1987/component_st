<template lang="html">
  <div>
    <Header />
    <MSlider />
    <Ada />
    <Money />
    <Adb />
    <Finance />
    <Adc />
    <Footor cname="mfooter"/>
    <Navbar />
  </div>
</template>

<script>
import Header from '../../js/public/header.vue'
import MSlider from './mslider.vue'
import Footor from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
import Ada from "./ada.vue"
import Money from "./money.vue"
import Adb from './adb.vue'
import Adc from './adc.vue'
import Finance from './finance.vue'
export default {
  components: { Header, MSlider, Footor, Navbar, Ada, Money, Adb, Adc, Finance }
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
