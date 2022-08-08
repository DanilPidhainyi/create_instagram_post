<template>
  <div class="post--container">
    <h3 class="post--title">
      <p>Ключові слова</p>
      <div class="line"></div>
    </h3>
    <article class="keyWords--container">
      <KeyWord id="1"/>
      <KeyWord id="2"/>
      <KeyWord id="3"/>
      <KeyWord id="4"/>
      <KeyWord id="5"/>
      <KeyWord id="6"/>
    </article>
    <article class="photoBar">
      <PhotoBar/>
    </article>
    <article class="sliders">
      <div>
        <p>Розмір фото</p>
      <Slider1/>
      </div>
      <div>
        <p>Кількість слів</p>
        <Slider2/>
      </div>
      <div>
        <p>Кількість тегів</p>
        <Slider2/>
      </div>
    </article>
  </div>
</template>

<script>
import KeyWord from "@/components/KeyWord";
import PhotoBar from "@/components/PhotoBar";

import 'vue-slider-component/theme/antd.css'
import Slider1 from "@/components/Slider1";
import Slider2 from "@/components/Slider2";
export default {
  name: "SettingsCom",
  components: {Slider2, Slider1, PhotoBar, KeyWord},
}

</script>

<style scoped>

.sliders {
  width: 100%;
  height: 230px;
  box-sizing: border-box;
  background-color: white;
  padding: 20px 10px;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}

.photoBar {
  margin: 20px 0;
}
.keyWords--container {
  padding-top: 10px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  align-content: start;
  height: 100%;
}

p {
  margin: 0;
  padding: 0 0 13px 0;
}

.post--title {
  padding: 0;
  margin: 0;
  font-family: 'Roboto', serif;
  font-style: normal;
  font-weight: 700;
  font-size: 25px;
}

.line {
  max-width: 100%;
  border-top: 1px dashed #000000;
  flex: none;
  order: 0;
  align-self: stretch;
  flex-grow: 0;
}

.post--title {
  max-width: 390px;
  height: 62px;
}

.post--container {
  margin: 0;
  padding: 27px 30px;
  width: 460px;
  height: 690px;
  box-sizing: border-box;
  background: rgba(227, 240, 243, 0.5);
  backdrop-filter: blur(20px);
  border-radius: 20px;
  display: flex;
  flex-direction: column;
}

</style>