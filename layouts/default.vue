<template>
  <div id="layout">
    <top-nav />

    <main
      id="main-view"
      role="main"
      aria-describedby="page-description"
    >
      <b-container fluid>
        <b-row>
          <b-col />
          <b-col
            xs="12"
            md="10"
          >
            <nuxt aria-busy="false" />
          </b-col>
          <b-col />
        </b-row>
      </b-container>
    </main>

    <!-- <footer /> -->
  </div>
</template>

<script>
import TopNav from '../components/TopNav.vue';
// import Footer from '../components/Footer.vue';
export default {
  components: {
    TopNav,
    // Footer,
  },
  data: () => ({ loading: true }),
  mounted() {
    if (!window.location.hash) {
      this.loading = false;
    }
  },
};
</script>

<style lang='scss'>
.success {
  color: green;
}
.error {
  color: red;
}
#layout {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
}
#main-view {
  flex: 1;
  margin: 1rem;
}
.btn {
  margin-left: 3px;
  margin-right: 3px;
  padding: .375rem .75rem;
}
/* Transitions */
.page-enter-active, .page-leave-active {
  transition: opacity .5s;
}
.page-enter, .page-leave-to {
  opacity: 0;
}
</style>