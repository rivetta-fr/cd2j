<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <a
          class="nav-link"
          href="/">
      <!-- <router-link class="navbar-brand" to="/"> -->
        <h3>CD2J</h3>
        
     </a>
      <!-- </router-link> -->
    </template>
    <template slot="navbar-menu">
      <li class="nav-item">
        <a
          class="nav-link"
          href="#experts">
          <h4>Expertises</h4>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          href="#team">
          <h4>Équipe</h4>
        </a>
      </li>
        <!-- <nav-link to="/landing">
          <i class="now-ui-icons education_paper"></i> Landing
        </nav-link> -->

      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Follow us on Twitter"
          data-placement="bottom"
          href="https://twitter.com/"
          target="_blank"
        >
          <i class="fab fa-twitter"></i>
          <p class="d-lg-none d-xl-none">Twitter</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Like us on Facebook"
          data-placement="bottom"
          href="https://www.facebook.com/"
          target="_blank"
        >
          <i class="fab fa-facebook-square"></i>
          <p class="d-lg-none d-xl-none">Facebook</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Like us on Linkedin"
          data-placement="bottom"
          href="https://www.linkedin.com/"
          target="_blank"
        >
          <i class="fab fa-linkedin"></i>
          <p class="d-lg-none d-xl-none">Linkedin</p>
        </a>
      </li>
    </template>
  </navbar>
</template>

<script>
import { Navbar } from '@/components';
import { Popover } from 'element-ui';
export default {
  name: 'main-navbar',
  props: {
    transparent: Boolean,
    colorOnScroll: Number
  },
  components: {
    Navbar,
    [Popover.name]: Popover
  }
};
</script>

<style scoped>

.nav-link h4 {
  margin-top: 0px;
  margin-bottom: 0px;
}

</style>
