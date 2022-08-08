<template>
  <div class="container">
    <input type="range" min="1" max="200" value="100" class="slider">
    <span class="number">00</span>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Slider2"
}
</script>

<style scoped>
.container {
  width: 100%;
  display: flex;
  align-items: center;
}

.number {
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
  margin: 0 10px;

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

.slider {
  width: 80%;
  cursor: pointer;
  opacity: 0.8;
  /*background-color: #E2E8F0;*/
  position: relative;
  /*-webkit-appearance: none;*/
  /*-moz-appearance: none;*/
  display: block;
  height: 4px;
  accent-color: #2563EB;
  border-radius: 8px;
  /*border: none;*/
  outline: none;
  z-index: 1;
  /*-webkit-appearance: none;*/
  /*background-color: #9a905d;*/
}

</style>