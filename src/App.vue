<script>
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"

export default {
  components: {
    TheHeader,
    TheFooter
  },
  data() {
    return {}
  }
}

</script>

<template>
  <div class="container-fluid px-0">
    <div class="row">
      <div class="col mx-auto">
        <TheHeader></TheHeader>
        <main>
          <a href="#">Link ad una pagina</a>
        </main>
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
