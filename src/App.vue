<template>
  <div id="App">
    <Personajes></Personajes>
  </div>
</template>

<script>
import Personajes from "./components/Personajes";
export default {
  name: "app",
  components: { Personajes },
};
</script>

<style lang="scss">
body {
  background-image: url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png);
  font-family: sans-serif;
}
</style>
