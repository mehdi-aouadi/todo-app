<template lang="pug">
  div(class="login")
    el-row(:span=12 class="center")
      el-col(:span=24)
          el-input(placeholder="Login" v-model="login" clearable)
    el-row(:span=12 class="center")
      el-col(:span=24)
        el-input(placeholder="password" type="password" clearable)
</template>

<script>
export default {
  name: 'Login',
  data() {
    return {
      login: '',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
  .center {
    margin: auto;
    width: 50%;
    padding: 10px;
}
</style>
