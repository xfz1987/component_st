<template lang="html">
  <div>
    <Header />
    <ISlider />
    <Welfare />
    <Service />
    <Footor/>
    <Navbar />
  </div>
</template>

<script>
import Header from '../../js/public/header.vue'
import ISlider from './islider.vue'
import Footor from '../public/footer.vue'
import Navbar from '../public/navbar.vue'
import Welfare from './welfare.vue'
import Service from './service.vue'
export default {
  components: { Header, ISlider, Footor, Navbar, Welfare, Service }
}
</script>
