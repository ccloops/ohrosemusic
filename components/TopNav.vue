<template>
  <nav
    role="navigation"
    toggleable="md"
    type="dark"
  >
    <nuxt-link class="nav-item" to="/">
      Home
    </nuxt-link>

    <nuxt-link class="nav-item" to="/music">
      Music
    </nuxt-link>

    <nuxt-link class="nav-item" to="/videos">
      Videos
    </nuxt-link>

    <nuxt-link class="nav-item" to="/tour">
      Tour
    </nuxt-link>

    <nuxt-link class="nav-item" to="/merch">
      Merch
    </nuxt-link>

    <iframe src="https://open.spotify.com/follow/1/?uri=spotify:artist:3k7ErvhO8cmFVOTrAVtuKe&size=detail&theme=light" width="300" height="56" scrolling="no" frameborder="0" style="border:none; overflow:hidden;" allowtransparency="true"></iframe>

    <nuxt-link class="nav-item" to="/admin">
      
    </nuxt-link>
  </nav>
</template>

<script>
export default {
}
</script>

<style scoped>
/* nav {
  background-color: #ab0000;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
  -webkit-box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
} */

.nav-item {
  text-decoration: none;
  color: red;
  font-size: 10em;
}
</style>
