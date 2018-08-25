<template>
  <div id="app" ref="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      clientHeight: ''
    }
  },
  mounted () {
    this.clientHeight = `${document.documentElement.clientHeight - 20}px`
    const that = this
    window.onresize = function temp () {
      that.clientHeight = `${document.documentElement.clientHeight - 20}px`
    }
  },
  watch: {
    clientHeight: function () {
      this.changeFixed(this.clientHeight)
    }
  },
  methods: {
    changeFixed (clientHeight) {
      this.$refs.app.style.height = clientHeight
    }
  }
}
</script>

<style>
</style>
