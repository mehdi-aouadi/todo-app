<template lang="pug">
  div Welcome to your Dashboard!

</template>

<script>
export default {
  name: 'Dashboard',
  data() {
    return {
      login: '',
    };
  },
  methods: {
    startHacking() {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'The login will be available soon!',
        duration: 5000,
      });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
</style>
