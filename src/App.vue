<template>
  <div id="app">
    <div id="nav" class="sticky-top">
      <nav class="navbar navbar-expand-sm navbar-light">
        <router-link to="/" class="text-light router-home-link">Home</router-link>
        <button class="navbar-toggler d-lg-none px-2 py-2" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
            aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse slideInLeft navbar-collapse" id="collapsibleNavId">
            <ul class="navbar-nav text-light mr-auto mt-2 mt-lg-0">
              <li class="nav-item ml-5">
                <router-link to="/about" class="text-light">About</router-link>
              </li>
              <li class="nav-item ml-5">
                <router-link to="/projects" class="text-light">Projects</router-link>
              </li>
            </ul>
            <li class="nav-item">
              <router-link to="/contact" class="text-light">Contact</router-link>
            </li>
        </div>
      </nav>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: 'Josefin Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: start;
  color: #2c3e50;
}
.navbar {
  background-color: #030303;
  padding: 20px 100px !important;
}
.router-home-link {
  color: #EA830C !important;
}
#nav a:hover {
  color: #EA830C !important;
}
.navbar-toggler {
  background-color: #121212 !important;
  border-radius: 12px;
}


@media only screen and (max-width: 768px) {
  .navbar {
    padding: 10px 25px !important;
  }
  .nav-item {
    margin-left: 0 !important;
    margin-top: 5px !important;
  }
  .slideInLeft {
  -webkit-animation-name: slideInLeft;
  animation-name: slideInLeft;
  -webkit-animation-duration: 1s;
  animation-duration: 1s;
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
  }
  @-webkit-keyframes slideInLeft {
  0% {
  -webkit-transform: translateX(-100%);
  transform: translateX(-100%);
  visibility: visible;
  }
  100% {
  -webkit-transform: translateX(0);
  transform: translateX(0);
  }
  }
  @keyframes slideInLeft {
  0% {
  -webkit-transform: translateX(-100%);
  transform: translateX(-100%);
  visibility: visible;
  }
  100% {
  -webkit-transform: translateX(0);
  transform: translateX(0);
  }
  }
}
</style>
