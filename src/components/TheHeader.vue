<template>
  <div>
    <nav class="navbar is-transparent">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="https://bulma.io/images/bulma-logo.png" alt="Bulma: a modern CSS framework based on Flexbox" width="112" height="28">
        </a>
        <div class="navbar-burger burger" data-target="navbarExampleTransparentExample">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>

      <div id="navbarExampleTransparentExample" class="navbar-menu">
        <!--<div class="navbar-start">-->
        <!--<a class="navbar-item" href="#">-->
        <!--Home-->
        <!--</a>-->
        <!--</div>-->
        <div class="navbar-end">
          <a class="navbar-item" href="#" @click="showLogin = true">
            Login
          </a>
        </div>
      </div>
    </nav>

    <modal-login v-show="showLogin" @close="showLogin = false"></modal-login>
  </div>
</template>

<script>
  import ModalLogin from './ModalLogin.vue'

  export default {
    name: 'TheHeader',
    components: {
      ModalLogin: ModalLogin
    },
    data: function(){
      return {
        showLogin: false
      }
    }
  }

  /* toggle hamburger menu */
  document.addEventListener('DOMContentLoaded', function () {
    // Get all "navbar-burger" elements
    var $navbarBurgers = Array.prototype.slice.call(document.querySelectorAll('.navbar-burger'), 0);

    // Check if there are any navbar burgers
    if ($navbarBurgers.length > 0) {

      // Add a click event on each of them
      $navbarBurgers.forEach(function ($el) {
        $el.addEventListener('click', function () {

          // Get the target from the "data-target" attribute
          var target = $el.dataset.target;
          var $target = document.getElementById(target);

          // Toggle the class on both the "navbar-burger" and the "navbar-menu"
          $el.classList.toggle('is-active');
          $target.classList.toggle('is-active');

        });
      });
    }
  });
</script>
