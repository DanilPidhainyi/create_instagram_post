<template>
  <div class="mainContainer">
    <SettingsCom/>
    <InstagramPost/>
  </div>
</template>

<script>

import InstagramPost from "@/components/InstagramPost";
import SettingsCom from "@/components/SettingsCom";
export default {
  el: '#app',
  name: 'App',
  components: {SettingsCom, InstagramPost},
}
</script>

<style>

.mainContainer {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: space-around;
  padding: 50px 0;
  box-sizing: border-box;
}


@media only screen and (min-width: 800px) {
  .mainContainer {
    padding-left: 0px;
    padding-right: 0px;

  }
}

@media only screen and (min-width: 1100px) {
  .mainContainer {
    padding-left: 50px;
    padding-right: 50px;

  }
}

@media only screen and (min-width: 1300px) {
  .mainContainer {
    padding-left: 150px;
    padding-right: 150px;

  }
}

body {
  background-color: #B1B0DF;
}

</style>