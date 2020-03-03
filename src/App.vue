<template>
  <div id="app">
    <Icon name="checked_in_bag_variation3-extra"></Icon>
    <Icon name="icon__bulb" width="40"></Icon>
    <Icon name="icon__tick" width="40" fill="red"></Icon>
    <Icon name="icon__tick" width="60" fill="green"></Icon>
    <Icon name="icon__tick" width="80" height="80" fill="blue" viewBox="0 0 24 24"></Icon>
  </div>
</template>

<script>
import Icon from "./components/Icon";

export default {
  name: "App",
  components: {
    Icon
  }
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
