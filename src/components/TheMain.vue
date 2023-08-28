<script>
import comicsList from "../db/comics";

export default {
  data() {
    return {
      comicsList
    };
  },
};
</script>

<template>
  <main>
    <div class="jumbotron-custom w-100 position-relative">
      <button class="btn btn-custom fw-bold fs-5 position-absolute px-4">CURRENT SERIES</button>
    </div>
    <div class="container-fluid cards-list">
      <div class="row">
        <div class="col-md-9 mx-auto px-0 d-flex justify-content-center flex-wrap">
          <div class="row row-cols-6 g-3">
            <div class="col" v-for="(comic, i) in comicsList" v-bind:key="`comic_${i}`">
              <div class="card border-0 rounded-0 bg-transparent">
                <img v-bind:src="comic.thumb" class="card-img-top rounded-0" alt="">
                <div class="card-body px-0">
                  <h5 class="text-white">
                    {{ comic.series }}
                  </h5>
                </div>
              </div>
            </div>
          </div>
          <button class="btn btn-custom fw-semibold">LEARN MORE</button>
        </div>
      </div>
    </div>
  </main>
  
</template>

<style lang="scss" scoped>

@use "../styles/partials/variables" as *;
@use "../styles/partials/button.scss" as *;

main{
  min-height: 390px;
}
.jumbotron-custom {
  background-image: url(../assets/img/jumbotron.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 360px;
  .btn {
    bottom: 0;
    left: 12%;
    transform: translateY(50%);
  }
}
.cards-list{
  min-height: 500px;
  padding-top: 3rem;
  padding-bottom: 1rem;
  background-color: $color-secondary;

  img {
    aspect-ratio: 1/1;
  }

  button {
    width: 180px;
  }
}

</style>