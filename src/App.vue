<template>
  <navbar v-if="!isRegisterPage"></navbar>
  <router-view></router-view>
</template>

<script>
export default {
  computed: {
    // Check if the current route is the register page
    isRegisterPage() {
      return this.$route.name === 'register'; // Adjust 'register' to your actual route name
    },
  },
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}


</style>
