<script>
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"
import TheMain from "./components/TheMain.vue"
import Banner from "./components/Banner.vue"

export default {
  components: {
    TheHeader,
    TheFooter,
    TheMain,
    Banner
  },
  data() {
    return {}
  }
}

</script>

<template>
  <div class="container-fluid px-0">
    <div class="row">
      <div class="col">
        <TheHeader></TheHeader>
        <TheMain></TheMain>
        <Banner></Banner>
        <TheFooter></TheFooter>
      </div>
    </div>
  </div>
</template>

<style>
main{
  background-image: url();
  padding-top: 3rem;
  padding-bottom: 3rem;
}
</style>
