<template>
    <div class="projects">
        <div class="fadeIn transparent-wrap">
          <h1>This is a projects page</h1>
        </div>
    </div>
</template>


<style scoped>
.projects {
  background-color: #030303 !important;
  background-attachment: fixed;
  min-height: 100vh;
  padding: 70px 100px !important;
  color: #fff;
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
    .projects {
      padding: 10px !important;
    }
    /* .about :nth-child(1) {
      padding-top: 30px !important;
      font-size: 60px;
      line-height: .9;
    } */
    /* .about p, .link {
      font-size: 17px !important;
    } */
    .transparent-wrap {
      background-color: rgba(255, 255, 255, 0.164);
      border-radius: 20px;
      padding: 10px !important;
      border: 1px solid #808080;
    }
  }
</style>