<template>
  <body>
  <div class="container-fluid content">
    <div class="container-fluid header">
      <logo /> 
      <!-- We can introduce same colour headline as the club website -->
      <h1 class="title">
        One<span class="highlighted">Stop</span>
      </h1>
      <h4 class="subtitle">
        In view to ease out the database management system for a company and to handle the data of the employees, co-workers, people attending seminars, conferences and workshops, etc. in a swift and easy-flow manner. Can be taken as a reference for further ideas and similar concepts henceforth.
      </h4>
      <div class="links">
        <a
          href="https://nitdgplug.org"
          target="_blank"
          class="button--green"
        >
          GLUG
        </a>
        <nuxt-link to="/login" class="button--grey">LogIn</nuxt-link> <!-- In the login section, we can say that only a  -->
      </div>
    </div>
    <div class="footer">
      <span>Created and Handled by :<br /></span> <h5>GNU/LINUX USER'S GROUP, NIT Durgapur</h5>
    </div>
  </div>
  </body>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.content {
  min-height: 100vh;
  width: 100%;
  background: rgb(34, 33, 33);
}
.container-fluid {
  padding: 0;
  margin: 0;
}
.header {
  position: relative;
  left:0;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 90%!important;
}
.footer {
  width: 90%!important;
  position: relative;
  justify-content: center;
  text-align: center;
  padding-top: 15%;
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 1000;
  font-size: 15px;
  word-spacing: 2px;
  padding-bottom: 15px;
  line-break: break-all;
}
.footer span {
  color: #fa631c;
}
.footer h5 {
  color: #528dcc;
}
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 4rem;
  color: #528dcc;
  letter-spacing: 1px;
}
span.highlighted {
  color: #fa631c;
}
.subtitle {
  font-weight: 300;
  font-size: 20px;
  color: #5c6f99;
  word-spacing: 5px;
  padding-bottom: 15px;
  margin-left: 5%;
}
.button
.links {
  padding-top: 15px;
}

@media only screen and (max-width: 374px) {
  .title {
    font-size: 2.5rem;
  }
}
</style>
