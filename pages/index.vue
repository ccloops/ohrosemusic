<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        Oh, Rose
      </h1>
      <img src="../assets/OhRose_SaskiaBaden.jpg" alt="">
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      title: 'Hello World!'
    }
  },
  head () {
    return {
      title: this.title,
      meta: [
        { hid: 'description', name: 'description', content: 'My custom description' },
        { rel: 'icon', type:'image/png', sizes: '32x32', href:'../assets/favicon-32x32.png' }
      ]
    }
  }
}
</script>

<style>
body {
  /* background-image: url('../assets/whilemyfathersleeps.jpg'); */
  background: lightGray;
}

h1, h2 {
  color: white;
}
</style>
