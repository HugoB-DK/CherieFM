<template>
  <div class="page-globale">
    <HeaderComponent />
    <Navbar />
    <HoroscopeComponent />
    <FooterComponent />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import HeaderComponent from '~/components/HeaderComponent.vue'
import FooterComponent from '~/components/FooterComponent.vue'
import HoroscopeComponent from '~/components/HoroscopeComponent.vue'

export default {
  name: 'IndexPage',
  components: { HeaderComponent, Navbar, HoroscopeComponent, FooterComponent }
}
</script>
<style>
.page-globale{
  min-height: 100vh;
}
</style>
