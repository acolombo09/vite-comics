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
      <div class="col-md-9 d-flex justify-content-start align-items-center py-4 mx-auto">
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
        <div class="col col-logo position-relative">
          <img src="../assets/img/dc-logo-bg.png" alt="logo-dc-bg">
        </div>
      </div>
    </div>
  </div>
  
  <div class="container-fluid px-0 footer-lower">
    <div class="row">
      <div class="col-md-9 d-flex justify-content-between align-items-center py-4 mx-auto">
        <div class="col-md-4 d-flex align-items-center justify-content-start">
          <button type="button" class="btn btn-lg btn-outline-primary border-2 rounded-0 text-white">SIGN-UP NOW!</button>
        </div>
        <ul class="nav col-md-4 d-flex justify-content-end align-items-center list-unstyled">
          <li class="ms-3"><a class="text-primary fs-5 fw-bold" href="#">FOLLOW US</a></li>
          <li class="ms-3"><a class="text-body-secondary" href="#"><img src="../assets/img/footer-facebook.png" alt="fb-footer"></a></li>
          <li class="ms-3"><a class="text-body-secondary" href="#"><img src="../assets/img/footer-twitter.png" alt="twitt-footer"></a></li>
          <li class="ms-3"><a class="text-body-secondary" href="#"><img src="../assets/img/footer-youtube.png" alt="yt-footer"></a></li>
          <li class="ms-3"><a class="text-body-secondary" href="#"><img src="../assets/img/footer-pinterest.png" alt="pint-footer"></a></li>
          <li class="ms-3"><a class="text-body-secondary" href="#"><img src="../assets/img/footer-periscope.png" alt="locator-footer"></a></li>
        </ul>
      </div>
    </div>
  </div>
  </footer>
</template>

<style lang="scss" scoped>

@use "../styles/partials/variables" as *;

a {
  text-decoration: none;
  color: $color-tertiary;
}

.footer-upper{
  // min-height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  .col-logo{
    min-height: 400px;
    overflow: hidden;
  }
  .logo-img{
    height: 130%;
    position: absolute;
    top: 50%;
    right: 0;
    transform: translateY(-50%);
  }
}

.footer-lower{
  background-color: $color-secondary;
}

.title {
  color: white;
}

</style>