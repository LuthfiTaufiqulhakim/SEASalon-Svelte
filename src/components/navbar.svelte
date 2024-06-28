<nav class="navbar relative-top">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">SEASalon</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
      <div class="navbar-toggler-icon">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </button>
    <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
      <div class="offcanvas-header">
        <h5 class="offcanvas-title" id="offcanvasNavbarLabel">Offcanvas</h5>
        <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
      </div>
      <div class="offcanvas-body">
        <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Dropdown
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li>
                <hr class="dropdown-divider">
              </li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
          </li>
        </ul>
        <form class="d-flex mt-3" role="search">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </div>
</nav>

<style>
  .navbar{
    box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.25);
  }
  .container-fluid{
    padding: 0px 40px 0px 40px;
    background-color: wheat;
  }
  /* navbar-toggler-icon */
.navbar-toggler-icon{
  width: 35px;
  height: 30px;
  margin: 10px 10px;
  position: relative;
  cursor: pointer;
  display: inline-block;
}
.navbar-toggler-icon span{
  background-color:#FFF;
  position: absolute;
  border-radius: 2px;
  transition: .3s cubic-bezier(.8, .5, .2, 1.4);
}
.navbar-toggler-icon span:nth-child(1){
  width: 100%;
  height:  4px;
  display: block;
  top: 0px;
  left: 0px;
}
.navbar-toggler-icon span:nth-child(2){
  width: 100%;
  height:  4px;
  display: block;
  top: 13px;
  left: 0px;
}
.navbar-toggler-icon span:nth-child(3){
  width: 100%;
  height:  4px;
  display: block;
  bottom: 0px;
  left: 0px;
}
.navbar-toggler-icon:not(.open):hover span:nth-child(1){
  width: 100%;
  height:  4px;
  display: block;
  top: -2px;
  left: 0px;
  transition: .3s cubic-bezier(.8, .5, .2, 1.4);
}
.navbar-toggler-icon:not(.open):hover span:nth-child(2){
  width: 100%;
  height:  4px;
  display: block;
  top: 13px;
  left: 0px;
  transition: .4s cubic-bezier(.8, .5, .2, 1.4);
}
.navbar-toggler-icon:not(.open):hover span:nth-child(3){
  width: 100%;
  height:  4px;
  display: block;
  bottom: -2px;
  left: 0px;
  transition: .3s cubic-bezier(.8, .5, .2, 1.4);
}
.navbar-toggler-icon.open {
  transform: rotate(-90deg);
}
.navbar-toggler-icon.open  span:nth-child(1){
  left:3px;
  top: 12px;
  width: 30px;
  transition: .3s cubic-bezier(.8, .5, .2, 1.4);
  transform: rotate(90deg);
  transition-delay: 150ms;
}
.navbar-toggler-icon.open  span:nth-child(2){
  left:2px;
  top: 20px;
  width: 20px;
  transition: .3s cubic-bezier(.8, .5, .2, 1.4);
  transform: rotate(45deg);
  transition-delay: 50ms;
}
.navbar-toggler-icon.open  span:nth-child(3){
  left:14px;
  top: 20px;
  width: 20px;
  transition: .3s cubic-bezier(.8, .5, .2, 1.4);
  transform: rotate(-45deg);
  transition-delay: 100ms;
}
.hero{
  margin-top: 200px;
}
.offcanvas{
  background-color: wheat;
}
</style>