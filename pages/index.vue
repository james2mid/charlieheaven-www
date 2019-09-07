<template>
  <section class="section">
    <CircleButton
      color="rgba(100, 100, 100, 0.7)"
      size="10vh"
      x="10%"
      y="62%"
      @click="click"
    />
  </section>
</template>

<script>
import CircleButton from '@/components/CircleButton.vue'

export default {
  name: 'Home',

  components: {
    CircleButton
  },

  methods: {
    click () {
      window.alert('That tickles! 😂')
    }
  }
}
</script>

<style>

html {
  min-height: 100vh;
  min-width: 100vw;
  background-color: black;
  background-image: url(https://progameguides.com/wp-content/uploads/2018/05/fortnite-1920x1080-wallpaper-season10-004.jpg);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  box-shadow: inset 0px 0px 100px 0px rgba(0,0,0,1);
}

</style>
