<template>
  <a
    class="circle heartbeat"
    :style="style"
    @click="$emit('click')"
  />
</template>

<script>
export default {
  name: 'CircleButton',

  props: {
    color: String,
    size: String,
    x: String,
    y: String
  },

  computed: {
    style () {
      return {
        backgroundColor: this.color,
        height: this.size,
        width: this.size,
        left: this.x,
        top: this.y,

      }
    }
  }
}
</script>

<style scoped>

.circle {
  position: absolute;
  display: block;
  border-radius: 50%;
}

</style>