<script>
export default {
  data() {
    return {
      navLinks: [
        { name: "CHARACTERS"},
        { name: "COMICS"},
        { name: "MOVIES"},
        { name: "TV"},
        { name: "GAMES"},
        { name: "COLLECTIBLES"},
        { name: "VIDEOS"},
        { name: "FANS"},
        { name: "NEWS"},
        { name: "SHOP"},
      ],
    };
  },
};
</script>

<template>
  <header class="bg-white py-3">
    <div class="row">
      <div class="col-md-9 d-flex justify-content-center align-items-center justify-content-between mx-auto px-0">
        <img src="../assets/img/dc-logo.png" alt="dc-logo-header">
        <ul class="nav nav-pills">
          <li class="nav-item" v-for="link in navLinks">
            <a href="#" class="nav-link">{{link.name}}</a></li>
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