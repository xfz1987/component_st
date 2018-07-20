<template lang="html">
    <div :class="$style.home">
      <Header />
      <HSlider />
      <Novice />
      <Borrow />
      <Money />
      <Product />
      <Life />
      <Footor/>
      <Navbar />
    </div>
</template>

<script>
import Header from '../../js/public/header.vue'
import HSlider from './hslider.vue'
import Novice from './novice.vue'
import Borrow from './borrow.vue'
import Money from './money.vue'
import Product from './product.vue'
import Life from './life.vue'
import Footor from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
export default {
  components: { Header, HSlider, Novice, Borrow, Money, Product, Life, Footor, Navbar }
}
</script>

<style lang="scss" module></style>
