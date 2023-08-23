<script>
export default {

}
</script>

<template>
  <header class="bg-white py-3">
    <div class="row">
      <div class="col-md-9 d-flex justify-content-center align-items-center justify-content-between mx-auto px-0">
        <img src="../assets/img/dc-logo.png" alt="dc-logo-header">
        <ul class="nav nav-pills">
          <li class="nav-item"><a href="#" class="nav-link">CHARACTERS</a></li>
          <li class="nav-item"><a href="#" class="nav-link">COMICS</a></li>
          <li class="nav-item"><a href="#" class="nav-link">MOVIES</a></li>
          <li class="nav-item"><a href="#" class="nav-link">TV</a></li>
          <li class="nav-item"><a href="#" class="nav-link">GAMES</a></li>
          <li class="nav-item"><a href="#" class="nav-link">COLLECTIBLES</a></li>
          <li class="nav-item"><a href="#" class="nav-link">VIDEOS</a></li>
          <li class="nav-item"><a href="#" class="nav-link">FANS</a></li>
          <li class="nav-item"><a href="#" class="nav-link">NEWS</a></li>
          <li class="nav-item"><a href="#" class="nav-link">SHOP</a></li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>

@use "../styles/partials/variables" as *;

header img {
  width: 72px;
}

header .nav-link {
  color: black;
}

li {
  position: relative;

}

li::after{
  content: "";
  position: absolute;
  left: 0;
  bottom: -2rem;
  height: 5px;
  width: 100%;
  background-color: $color-primary;
  scale: 0 1;
  transition: scale 250ms;
}

li:hover::after{
  scale: 1 1;
}

a:hover,
a:focus-visible {
  color: $color-primary;
}

</style>