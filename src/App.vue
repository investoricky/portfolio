<template>
  <div id="app">
    <div id="nav" class="sticky-top">
      <nav class="navbar navbar-expand-sm navbar-light">
        
        <button class="navbar-toggler d-lg-none px-2 py-2 ml-auto" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
            aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"><i class="fa fa-bars px-3 py-3" aria-hidden="true"></i></span>
        </button>
        <div class="collapse slideInLeft navbar-collapse" id="collapsibleNavId">
            
            <ul class="navbar-nav text-light mr-auto mt-2 mt-lg-0">
              <router-link to="/" class="text-light router-home-link">Home</router-link>
              <li class="nav-item ml-5">
                <router-link to="/about" class="text-light">About</router-link>
              </li>
              <li class="nav-item ml-5">
                <router-link to="/projects" class="text-light">Projects</router-link>
              </li>
              <li class="nav-item ml-5">
                <router-link to="/contact" class="text-light">Contact</router-link>
              </li>
            </ul>
            <li class="nav-item">
              <p class="text-light link">{{ time }}</p>
            </li>
        </div>
      </nav>
    </div>
    <router-view/>
  </div>
</template>

<script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.1/moment-with-locales.min.js"></script>
<script>
export default {
  name: 'navbar',
  data() {
    return {
      time: '',
    }
  },
  methods: {
    showTime: function() {
      const m = moment();
      m.locale('en-au');
      this.time = (m.format('llll'));
    }
  },
  mounted: function() {
    this.showTime()
  }
}
</script>

<style>
* {
  margin: 0 !important;
  padding: 0 !important;
  list-style-type: none;
  text-decoration: none !important;
  line-height: 1.2;
  outline: none !important;
}
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
.fa-bars {
  background-color: rgba(255, 255, 255, 0.164);
  border-radius: 12px;
}
.link {
    color: #EA830C !important;
  }


@media only screen and (max-width: 768px) {
  .navbar {
    padding: 10px 25px !important;
  }
  .nav-item {
    margin-left: 0 !important;
    margin-top: 5px !important;
  }
  /* .navbar-nav {
    height: 100vh;
    width: 100%;
    align-items: center;
    display: none;
  } */
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
  .link {
    color: #fff !important;
  }
}
</style>
