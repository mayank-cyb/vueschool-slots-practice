<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <AppButton @click="useMe">Use me</AppButton>
  <AppButton>Like me</AppButton>
  <AppButton>Buy me</AppButton>
</template>

<script>
import AppButton from './components/AppButton.vue';

export default {
  name: 'App',
  components: {
    AppButton,
  },
  methods: {
    useMe() {
      console.log("Clicked use me");
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
