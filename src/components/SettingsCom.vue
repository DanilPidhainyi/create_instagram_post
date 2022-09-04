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
      <div class="slider--one" >
        <p>Розмір фото</p>
        <el-slider
            v-model="numberOfImgSize"
            max="200"
            input-size="small"
            size="small"
            class="slider"
            :marks="marks"
        />
      </div>
      <div>
        <p>Кількість слів</p>
        <div class="slider2__container">
          <el-slider
              v-model="numberOfWords"
              input-size="small"
              class="slider"
          />
          <span class="slider2__number">{{ numberOfWords }}</span>
        </div>
      </div>
      <div>
        <p>Кількість тегів</p>
        <div class="slider2__container">
          <el-slider
              v-model="numberOfTags"
              input-size="small"
              class="slider"
          />
          <span class="slider2__number">{{ numberOfTags }}</span>
        </div>
      </div>
    </article>
  </div>
</template>

<script>
import KeyWord from "@/components/KeyWord";
import PhotoBar from "@/components/PhotoBar";

const marks = {
  0: {
    style: {
      color: '#153789',
      paddingLeft: '10px'
    },
    label: '0',
  },
  50: '50',
  100: {
    style: {
      color: '#153789',
    },
    label: '100',
  },
  150: '150',
  200: {
    style: {
      color: '#153789',
      paddingRight: '20px'
    },
    label: '200',
  },

}


export default {
  name: "SettingsCom",
  components: { PhotoBar, KeyWord },
  data() {
    return {
      numberOfImgSize: 100,
      numberOfTags: 5,
      numberOfWords: 20,
      marks: marks
    }
  },
}
</script>


<style scoped>

.slider--one {
  margin-bottom: 20px;
}

.slider {
  /*--el-slider-main-bg-color: var(--color-slider)*/
}

.slider2__container {
  padding-left: 5px;
  width: 100%;
  display: flex;
  align-items: center;
}

.slider2__number {
  box-sizing: border-box;

  /* Auto layout */

  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 4px 20px;
  gap: 4px;

  max-width: 30px;
  width: max-content;
  height: 24px;
  margin: 0 5px 0 12px;

  /* white/white */

  background: #FFFFFF;
  /* gray/300 */

  border: 1px solid #CBD5E1;
  border-radius: 2px;

  /* Inside auto layout */

  flex: none;
  order: 0;
  flex-grow: 1;
}


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