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
    
  </main>
  <div class="container-fluid cards-list">
      <div class="row">
        <div class="col-md-9 mx-auto px-0">
          <div class="row row-cols-6 g-3">
            <div class="col" v-for="(comic, i) in comicsList" v-bind:key="`comic_${i}`">
              <div class="card border-0 rounded-0">
                <img v-bind:src="comic.thumb" class="card-img-top" alt="">
                <div class="card-body">
                  <h5 class="card-title">
                    {{ comic.series }}
                  </h5>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<style lang="scss" scoped>

@use "../styles/partials/variables" as *;

main{
  min-height: 390px;
  padding-top: 3rem;
  padding-bottom: 3rem;
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

.cards-list{
  min-height: 500px;
  padding-top: 3rem;
  padding-bottom: 3rem;
  background-color: $color-secondary;
}

.card {
  width: 120px;
  height: 120px;
}

</style>