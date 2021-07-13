<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <router-link to="/mentions">
              Mentions Légales
            </router-link>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, Designed and Coded by 
        <a href="/" target="_blank" rel="noopener"
          >CD2J</a
        >.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>