<script>
export default {
  data() {
    return {
      DcComicsLinks: [
        { name: "Characters"},
        { name: "Comics" },
        { name: "Movies"},
        { name: "Tv"},
        { name: "Games"},
        { name: "Videos"},
        { name: "News"},
        ],
      ShopLinks:[
        { name: "Shop Dc"},
        { name: "Shop Collectables" },
        ],
      DCLinks:[
        { name: "Terms Of Use"},
        { name: "Privacy Policy(New)" },
        { name: "AdChoice"},
        { name: "Advertising"},
        { name: "Jobs"},
        { name: "Subscriptions"},
        { name: "Talent Workshops"},
        { name: "CPSC Certificates"},
        { name: "Ratings"},
        { name: "Shop Help"},
        { name: "Contact Us"},
        ],
      SitesLinks:[
        { name: "DC"},
        { name: "Mad Magazine"},
        { name: "DC Kids"},
        { name: "DC Universe"},
        { name: "DC Power Visa"},
        ],
    }
  }
}
</script>

<template>
  <footer>
  <div class="container-fluid px-0 footer-upper">
    <div class="row mx-0">
      <div class="col-md-4 d-flex justify-content-between px-0">
        <div class="row mx-0">
          <div class="col-4 px-0">
            <h6 class="title">DC COMICS</h6>
            <ul class="list-unstyled">
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h6 class="title">SHOP</h6>
            <ul class="list-unstyled">
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col-4 px-0">
            <h6 class="title">DC</h6>
            <ul class="list-unstyled">
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="col-4 px-0">
            <h6 class="title">SITES</h6>
            <ul class="list-unstyled">
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div> 
      </div>
    </div>
  </div>
  
  <div class="container">
    <div class="d-flex flex-wrap justify-content-between align-items-center py-3 my-4 border-top">
      <div class="col-md-4 d-flex align-items-center">
        <a href="/" class="mb-3 me-2 mb-md-0 text-body-secondary text-decoration-none lh-1">
          <svg class="bi" width="30" height="24"><use xlink:href="#bootstrap"></use></svg>
        </a>
        <span class="mb-3 mb-md-0 text-body-secondary">© 2023 Company, Inc</span>
      </div>

      <ul class="nav col-md-4 justify-content-end list-unstyled d-flex">
        <li class="ms-3"><a class="text-body-secondary" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#twitter"></use></svg></a></li>
        <li class="ms-3"><a class="text-body-secondary" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#instagram"></use></svg></a></li>
        <li class="ms-3"><a class="text-body-secondary" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#facebook"></use></svg></a></li>
      </ul>
    </div>
  </div>

  <div class="container-fluid px-0 footer-lower">
    <div class="row mx-0">
      <div class="col-md-4 d-flex justify-content-between px-0">
        <div class="row mx-0">
          <div class="col px-0">
            <h6 class="title">DC COMICS</h6>
            <ul class="list-unstyled">
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
            </ul>
          </div>
          <div class="col px-0">
            <h6 class="title">DC</h6>
            <ul class="list-unstyled">
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
            </ul>
          </div>
        </div> 
      </div>
    </div>
  </div>
  </footer>
</template>

<style lang="scss" scoped>

@use "../styles/partials/variables" as *;

// footer {
  
// }

a {
  text-decoration: none;
  color: $color-tertiary;
}

.footer-upper{
  background-image: url(../assets/img/footer-bg.jpg);
}

.footer-lower{
  background-color: $color-secondary;
}

.title {
  color: white;
}

</style>