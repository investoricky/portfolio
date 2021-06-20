<template>
  <div class="about">
    <div class="fadeIn transparent-wrap">
      <h1>I build value by <br> design.</h1>
      <p class="text-muted mt-3">I’m Nsisong Akpan, but you can just call me Ricky.</p>
      <p class="text-muted mt-3">
        Originally hailing from Akwa-Ibom State, Nigeria. For the last <br> Three(3) Years or so I’ve been honing my skills in design, 
        production <br> and management roles, building products for the web and mobile etc.
      </p>
      <p class="text-muted mt-3">
        I strive to create elegant solutions that surprise and delight users, <br> while keeping complex technical dependencies in mind for <br> 
        implementation, scalability and developer sanity.
      </p>
      <p class="text-muted mt-3">
        I’ve worked with small, agile teams on start innovation hub projects <br> with product lifecycles spanning multiple years.
      </p>
      <p class="text-muted mt-3">
        Depending on the team, resources and deliverables I’ve worn many <br> hats over the years - holding titles like Product Designer, 
        UI Designer, <br> UX Designer, Front-end Developer, & Product Manager.
      </p>
      <p class="text-muted mt-3">I also occasionally give talks on design and product development.</p>
      <p class="text-muted mt-3">Have an interesting project? <router-link to="/contact" class="link">Let's talk.</router-link></p>
    </div>
  </div>
</template>

<style scoped>
.about {
  background-color: #030303 !important;
  background-attachment: fixed;
  min-height: 100vh;
  padding: 70px 100px !important;
  color: #fff;
}
.about :nth-child(1) {
  font-size: 70px;
  color: #EA830C;
}
  .about p, .link {
    font-size: 25px !important;
  }
  .link {
    color: #EA830C;
  }
.fadeIn {
  -webkit-animation-name: fadeIn;
  animation-name: fadeIn;
  -webkit-animation-duration: 3s;
  animation-duration: 3s;
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


  @media only screen and (max-width: 768px) {
    .about {
      padding: 10px !important;
    }
    .about :nth-child(1) {
      padding-top: 30px !important;
      font-size: 60px;
      line-height: .9;
    }
    .about p, .link {
      font-size: 17px !important;
    }
    .transparent-wrap {
      background-color: rgba(255, 255, 255, 0.164);
      border-radius: 20px;
      padding: 10px !important;
      border: 1px solid #808080;
    }
  }
</style>