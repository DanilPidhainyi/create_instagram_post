<template>
  <div class="container">
    <input type="range" min="1" max="200" value="100" class="slider">
    <div class="point--container">
      <div class="point"/>
      <div class="point"/>
      <div class="point"/>
      <div class="point"/>
      <div class="point"/>
    </div>
    <div class="number--container">
      <div class="number">0</div>
      <div class="number">50</div>
      <div class="number">100</div>
      <div class="number">150</div>
      <div class="number">200</div>
    </div>

  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Slider1"
}
</script>

<style scoped>

.number--container {
  width: 100%;
  box-sizing: border-box;
  display: flex;
  justify-content: space-between;
}

.number {
  width: 20px;
}

.point--container {
  width: 100%;
  box-sizing: border-box;
  padding: 0 0 0 2px;
  position: relative;
  bottom: 6px;
  display: flex;
  justify-content: space-between;
}

.point {
  width: 4px;
  height: 4px;
  background-color: rgb(0, 0, 0);
  border-radius: 50%;
}


.slider {
  width: 100%;
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



/*.slider::-webkit-slider-runnable-track {*/
/*  height: 10px;*/
/*  -webkit-appearance: none;*/
/*  color: #13bba4;*/
/*  margin-top: -1px;*/
/*}*/

/*.slider::-webkit-slider-thumb {*/
/*  width: 10px;*/
/*  -webkit-appearance: none;*/
/*  height: 10px;*/
/*  cursor: ew-resize;*/
/*  background: #434343;*/

/*  box-shadow: -80px 0 0 80px #43e5f7;*/
/*  border-radius: 50%;*/
/*}*/

/*.slider::-moz-range-progress {*/
/*  background-color: #43e5f7;*/
/*}*/
/*.slider::-moz-range-track {*/
/*  background-color: #9a905d;*/
/*}*/
/*.slider::-ms-fill-lower {*/
/*  background-color: #43e5f7;*/
/*}*/
/*.slider::-ms-fill-upper {*/
/*  background-color: #9a905d;*/
/*}*/

/*.slider::-ms-track{*/
/*  appearance: none;*/
/*  height: 8px;*/
/*}*/

/*.slider::-webkit-slider-thumb {*/
/*  -webkit-appearance: none;*/
/*  height: 20px;*/
/*  width: 20px;*/
/*  background-color: blue;*/
/*  border-radius: 50%;*/
/*  !*pointer-events: auto;*!*/
/*  cursor: pointer;*/
/*  margin-top: -6px;*/
/*  border: none;*/
/*}*/

/*.slider::-moz-range-thumb {*/
/*  -webkit-appearance: none;*/
/*  height: 20px;*/
/*  width: 20px;*/
/*  background-color: blue;*/
/*  border-radius: 50%;*/
/*  !*pointer-events: auto;*!*/
/*  cursor: pointer;*/
/*  margin-top: -6px;*/
/*  border: none;*/
/*}*/

/*.slider::-ms-thumb {*/
/*  appearance: none;*/
/*  height: 20px;*/
/*  width: 20px;*/
/*  background-color: blue;*/
/*  border-radius: 50%;*/
/*  !*pointer-events: auto;*!*/
/*  cursor: pointer;*/
/*  margin-top: -6px;*/
/*  border: none;*/
/*}*/

/*.slider:active::-webkit-slider-thumb {*/
/*  background-color: white;*/
/*  border: 3px solid blue;*/
/*}*/
/*.slider:hover {*/
/*  opacity: 1;*/
/*}*/


.container {
  width: 100%;
  box-sizing: border-box;
  padding: 0 5px;
  /*background-color: #ec0049;*/
}
</style>