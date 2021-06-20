<template>
  <div class="home">
    <div class="fadeIn transparent-wrap">
      <h2 class="text-muted">Hi, I'm Nsisong Akpan.</h2>
      <p class="mt-5">A Web Developer, <br> Product Person.</p>
      <p class="text-muted mt-2">Multidisciplinary Designer who strives at developing web apps, <br> building and customization of websites.</p>
      <p class="text-muted mt-3">Less moody in real life. <i class="fa fa-thumbs-up" aria-hidden="true"></i></p>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import projects from '@/components/Contact'

export default {
  data() {
    return{}
  },
  // components: {
  //   projects
  // }
}
</script>

<style scoped>
  .home {
    background-color: #030303 !important;
    background-attachment: fixed;
    min-height: 100vh;
    padding: 150px 100px !important;
    color: #fff;
  }
  .home :nth-child(2) {
    font-size: 70px;
    color: #EA830C;
  }
  .home :nth-child(3), .home :nth-child(4) {
    font-size: 25px;
  }
  .fa-thumbs-up {
    color: #FFC83D;
  }
  .fadeIn {
  -webkit-animation-name: fadeIn;
  animation-name: fadeIn;
  -webkit-animation-duration: 5s;
  animation-duration: 5s;
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
  }
  @-webkit-keyframes fadeIn {
  0% {opacity: 0;}
  100% {opacity: 1;}
  }
  @keyframes fadeIn {
  0% {opacity: 0;}
  100% {opacity: 1;}
  } 

  @keyframes fadeInUp {
  0% {
  opacity: 0;
  -webkit-transform: translate3d(0, 100%, 0);
  transform: translate3d(0, 100%, 0);
  }
  100% {
  opacity: 1;
  -webkit-transform: none;
  transform: none;
  }
  } 

  @media only screen and (max-width: 768px) {
    .home {
      padding: 10px !important;
    }
    .transparent-wrap {
      background-color: rgba(255, 255, 255, 0.164);
      border-radius: 20px;
      padding: 10px !important;
      border: 1px solid #808080;
    }
    .home :nth-child(2) {
      font-size: 45px;
      line-height: 1;
    }
    .home :nth-child(1) {
      padding-top: 30px !important;
    }
    .home :nth-child(1), .home :nth-child(3), .home :nth-child(4) {
    font-size: 18px;
    }
  }
</style>
