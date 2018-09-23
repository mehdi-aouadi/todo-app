<template lang="pug">
  div(class="login")
    el-row(:span=12 class="center")
      el-col(:span=24)
          el-input(placeholder="Login" v-model="login" clearable)
    el-row(:span=12 class="center")
      el-col(:span=24)
        el-input(placeholder="password" type="password" clearable)
    el-row(:span=12 class="center")
      el-col(:span=24)
        el-button(type="primary"  @click="startHacking" style="width: 100px;") Login
    el-row(:span=12 class="center")
      el-col(:span=24)
        el-button(type="primary" style="width: 100px;") New User
</template>

<script>
export default {
  name: 'Login',
  data () {
    return {
      login: ''
    }
  },
  methods: {
    startHacking () {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
  .center {
    margin: auto;
    width: 50%;
    padding: 10px;
}
</style>
