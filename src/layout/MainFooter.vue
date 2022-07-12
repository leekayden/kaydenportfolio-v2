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
            <a href="https://portfolio.kaydentech.com">
              Kayden Lee
            </a>
          </li>
          <li>
            <a href="https:///presentation.portfolio.kaydentech.com">
              About Us
            </a>
          </li>
          <li>
            <a href="https:///blog.portfolio.kaydentech.com">
              Blog
            </a>
          </li>
          <li>
            <a href="https://portfolio.kaydentech.com/license">
              Licenses
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, made with <md-icon>favorite</md-icon> by
        <a href="/" target="_blank">Kayden Lee</a>
        for a better web.
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
