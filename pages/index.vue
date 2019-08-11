<template>
  <div class="content">
    <header>
    </header>
    <article class="center">
      <section>
        <h1 class="jp">どうも！<br/>ペドロです</h1>
        <p class="upper tagline">Web Developer, Scuba Divemaster, Nomad</p>
      </section>
      <figure>
        <img src="~/assets/itsme.jpg">
      </figure>
      <section>
        <h4 class="jp">システムエンジニアのペドロです</h4>
      </section>
      <section>
        <p class="intro">{{ intro }}</p>
      </section>
      <section>
        <p class="work"><nuxt-link to="/contact">{{ work }}</nuxt-link></p>
      </section>
      <section>
        <h2 class="headlight">Tell me more</h2>
        <p class="intro">{{ tellmemore }}</p>
      </section>
      <section>
        <h2 class="headlight">Where are you?</h2>
        <p class="intro">I'm currently anchored in Akita, Japan. Working on developing <a href="https://www.tanehub.asia/" target="_blank">TANEHUB</a> and growing the community around it.</p>
      </section>
      <section>
        <h2 class="headlight">Any projects?</h2>
        <p class="intro projects"><a class="joblink-green" href="http://mountainviewresidence.ro/" target="_blank">Mountain View Residence</a>. <a class="joblink-blue" href="http://tanehub.asia/" target="_blank">TANEHUB.</a> <a class="joblink-yellow" href="https://github.com/pedrogaudencio/arduino-rpi" target="_blank">Arduino Raspberry Pi.</a> <a class="joblink-red" href="https://www.arpropertythailand.com/" target="_blank">AR Property Thailand</a>. <a class="joblink-blue" href="https://github.com/pedrogaudencio/algae-notify" target="_blank">Algae Monitoring.</a> <a class="joblink-orange" href="https://github.com/inveniosoftware/invenio" target="_blank">Invenio.</a> <a class="joblink-yellow" href="https://github.com/indico/indico" target="_blank">Indico.</a> <a class="joblink-pink" href="http://www.chjtech.com.sg/" target="_blank">CHJ Tech.</a> <a class="joblink-turquoise" href="https://github.com/rufuspollock/markdown2latex" target="_blank">Markdown2Latex.</a></p>
      </section>
      <section>
        <ul id="social">
          <li><a href="mailto:me@watashipedro.com"><svg width="35" height="35" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" data-svg="mail"><polyline fill="none" stroke="#000" points="1.4,6.5 10,11 18.6,6.5"></polyline><path d="M 1,4 1,16 19,16 19,4 1,4 Z M 18,15 2,15 2,5 18,5 18,15 Z"></path></svg></a></li>
          <li><a href="https://www.linkedin.com/in/pedrogaudencio" target="_blank"><svg width="35" height="35" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" data-svg="linkedin"><path d="M5.77,17.89 L5.77,7.17 L2.21,7.17 L2.21,17.89 L5.77,17.89 L5.77,17.89 Z M3.99,5.71 C5.23,5.71 6.01,4.89 6.01,3.86 C5.99,2.8 5.24,2 4.02,2 C2.8,2 2,2.8 2,3.85 C2,4.88 2.77,5.7 3.97,5.7 L3.99,5.7 L3.99,5.71 L3.99,5.71 Z"></path><path d="M7.75,17.89 L11.31,17.89 L11.31,11.9 C11.31,11.58 11.33,11.26 11.43,11.03 C11.69,10.39 12.27,9.73 13.26,9.73 C14.55,9.73 15.06,10.71 15.06,12.15 L15.06,17.89 L18.62,17.89 L18.62,11.74 C18.62,8.45 16.86,6.92 14.52,6.92 C12.6,6.92 11.75,7.99 11.28,8.73 L11.3,8.73 L11.3,7.17 L7.75,7.17 C7.79,8.17 7.75,17.89 7.75,17.89 L7.75,17.89 L7.75,17.89 Z"></path></svg></a></li>
          <li><a href="https://github.com/pedrogaudencio/" target="_blank"><svg width="35" height="35" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" data-svg="github-alt"><path d="M10,0.5 C4.75,0.5 0.5,4.76 0.5,10.01 C0.5,15.26 4.75,19.51 10,19.51 C15.24,19.51 19.5,15.26 19.5,10.01 C19.5,4.76 15.25,0.5 10,0.5 L10,0.5 Z M12.81,17.69 C12.81,17.69 12.81,17.7 12.79,17.69 C12.47,17.75 12.35,17.59 12.35,17.36 L12.35,16.17 C12.35,15.45 12.09,14.92 11.58,14.56 C12.2,14.51 12.77,14.39 13.26,14.21 C13.87,13.98 14.36,13.69 14.74,13.29 C15.42,12.59 15.76,11.55 15.76,10.17 C15.76,9.25 15.45,8.46 14.83,7.8 C15.1,7.08 15.07,6.29 14.75,5.44 L14.51,5.42 C14.34,5.4 14.06,5.46 13.67,5.61 C13.25,5.78 12.79,6.03 12.31,6.35 C11.55,6.16 10.81,6.05 10.09,6.05 C9.36,6.05 8.61,6.15 7.88,6.35 C7.28,5.96 6.75,5.68 6.26,5.54 C6.07,5.47 5.9,5.44 5.78,5.44 L5.42,5.44 C5.06,6.29 5.04,7.08 5.32,7.8 C4.7,8.46 4.4,9.25 4.4,10.17 C4.4,11.94 4.96,13.16 6.08,13.84 C6.53,14.13 7.05,14.32 7.69,14.43 C8.03,14.5 8.32,14.54 8.55,14.55 C8.07,14.89 7.82,15.42 7.82,16.16 L7.82,17.51 C7.8,17.69 7.7,17.8 7.51,17.8 C4.21,16.74 1.82,13.65 1.82,10.01 C1.82,5.5 5.49,1.83 10,1.83 C14.5,1.83 18.17,5.5 18.17,10.01 C18.18,13.53 15.94,16.54 12.81,17.69 L12.81,17.69 Z"></path></svg></a></li>
          <li><a href="https://www.couchsurfing.com/people/pedrogaudencio" target="_blank"><svg width="35" height="35" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" data-svg="world"><path fill="none" stroke="#000" d="M1,10.5 L19,10.5"></path><path fill="none" stroke="#000" d="M2.35,15.5 L17.65,15.5"></path><path fill="none" stroke="#000" d="M2.35,5.5 L17.523,5.5"></path><path fill="none" stroke="#000" d="M10,19.46 L9.98,19.46 C7.31,17.33 5.61,14.141 5.61,10.58 C5.61,7.02 7.33,3.83 10,1.7 C10.01,1.7 9.99,1.7 10,1.7 L10,1.7 C12.67,3.83 14.4,7.02 14.4,10.58 C14.4,14.141 12.67,17.33 10,19.46 L10,19.46 L10,19.46 L10,19.46 Z"></path><circle fill="none" stroke="#000" cx="10" cy="10.5" r="9"></circle></svg></span></a></li>
          <li><a href="https://www.facebook.com/pedrogaudencio" target="_blank"><svg width="35" height="35" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" data-svg="facebook"><path d="M11,10h2.6l0.4-3H11V5.3c0-0.9,0.2-1.5,1.5-1.5H14V1.1c-0.3,0-1-0.1-2.1-0.1C9.6,1,8,2.4,8,5v2H5.5v3H8v8h3V10z"></path></svg></a></li>
          <li><a href="https://www.instagram.com/pedrogaudencio/" target="_blank"><svg width="35" height="35" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" data-svg="instagram"><path d="M13.55,1H6.46C3.45,1,1,3.44,1,6.44v7.12c0,3,2.45,5.44,5.46,5.44h7.08c3.02,0,5.46-2.44,5.46-5.44V6.44 C19.01,3.44,16.56,1,13.55,1z M17.5,14c0,1.93-1.57,3.5-3.5,3.5H6c-1.93,0-3.5-1.57-3.5-3.5V6c0-1.93,1.57-3.5,3.5-3.5h8 c1.93,0,3.5,1.57,3.5,3.5V14z"></path><circle cx="14.87" cy="5.26" r="1.09"></circle><path d="M10.03,5.45c-2.55,0-4.63,2.06-4.63,4.6c0,2.55,2.07,4.61,4.63,4.61c2.56,0,4.63-2.061,4.63-4.61 C14.65,7.51,12.58,5.45,10.03,5.45L10.03,5.45L10.03,5.45z M10.08,13c-1.66,0-3-1.34-3-2.99c0-1.65,1.34-2.99,3-2.99s3,1.34,3,2.99 C13.08,11.66,11.74,13,10.08,13L10.08,13L10.08,13z"></path></svg></a></li>
      </ul>
      </section>
    </article>
  </div>
</template>

<script>
  // import Intro from '../components/intro.vue';
  import Parallax from "vue-parallaxy";

  export default {
    components: {
      Parallax
    },
    data: () => ({
      profile: '',
      intro: 'Hi, I\'m Pedro. Most of the time I create websites and web applications.',
      work: 'Let\'s work together',
      tellmemore: 'Born in Portugal, made the world my home and moved from one country to the next. Shifting between working remotely as a freelance web developer and graphic designer and volunteering in several projects around Europe and Asia, keeping the slow travel mindset I\'ve been able to prolong an overland trip from Singapore to Portugal since 2015.',
    })
  }
</script>

<style>
html {
  background: #fafafa;
  color: #000;
  /*font-family: 'Montserrat', sans-serif;*/
  font-family: Roboto, sans-serif;
  scroll-behavior: smooth;
}

.content {
  display: grid;
  grid-template-columns: 
  [full-start] minmax(1em, 1fr) 
  [main-start] minmax(0, 106em) [main-end]
  minmax(1em, 1fr) [full-end];
  grid-gap: 1em;
}

section {
  grid-column: main;
}

figure {
  grid-column: full;
}

article > * {
  background-color: #fff;
  padding: 2em;
}

figure {
  text-align: center;
}

img {
  max-width: 100%;
}

body {
  margin: 50px auto;
  max-width: 100%;
  min-width: 375px;
  padding: .5em 1em;
}

header {
}

h1 {
  display: inline;
  font-size: 9em;
}

h3 {
  font-size: 6em;
  font-weight: 100;
}

h4 {
  font-size: 3.8em;
  padding-top: 5vw;
}

p {
  font-size: 1em;
}

a {
  color: #000;
  text-decoration: none;
  border-bottom: dotted .1em #818479;
}

.joblink-red {
  border-bottom: dashed .1em #ed3700;
}

.joblink-blue {
  border-bottom: dashed .1em #5f8fc6;
}

.joblink-yellow {
  border-bottom: dashed .1em #f3de8a;
}

.joblink-green {
  border-bottom: dashed .1em #cae7b9;
}

.joblink-orange {
  border-bottom: dashed .1em #d89d6a;
}

.joblink-pink {
  border-bottom: dashed .1em #af3b6e;
}

.joblink-turquoise {
  border-bottom: dashed .1em #bce7fd;
}

.jp {
  font-family: 'Noto Sans JP', sans-serif;
}

.intro {
  margin: auto auto;
  padding-top: 10vw;
  max-width: 11em;
  font-size: 5vw;
  text-align: left;
  line-height: 1.3;
  transition: .4s ease;
}

.tagline {
  padding-top: 5vw;
  padding-bottom: 5vw;
}

.upper {
  text-transform: uppercase;
}

.center {
  text-align: center;
}

.headlight {
  text-align: left;
  padding-top: 20vw;
  padding-bottom: 1em;
  max-width: 11em;
  font-size: 11vw;
  transition: .4s ease;
}

.projects {
  font-size: 8vw;
}

.mobile-only {
  display: none;
}

#social {
  list-style: none;
  margin-top: 10vw;
}

#social > li {
  display: inline;
  float: left;
}

#social > li > a {
  border-bottom: none;
  padding-right: 1.2vw;
}

#social > li:first-child {
  margin-top: 5px;
}

@media only screen and (max-width: 414px) {
  body {
    padding: .5em;
    margin: 0;
  }
  article > * {
    padding: 0em;
  }
  h1 {
    font-size: 3.3em;
    font-weight: 400;
    padding-bottom: .5em;
  }
  h4 {
    font-size: 1em;
  }
  p {
    margin-top: 20px;
    padding: .4em .3em;
  }
  .projects {
    line-height: 1.8;
  }
  .headlight {
    font-size: 2.2em;
    line-height: 1.8;
    text-align: left !important;
  }
  .intro {
    padding-top: 2vw;
  }
  .mobile-none {
    display: none;
  }
  .mobile-only {
    display: inline;
  }
}

</style>
