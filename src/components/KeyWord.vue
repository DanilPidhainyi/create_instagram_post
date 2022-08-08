<template>
  <form class="container">
    <div class="checkbox--container">
      <input type="checkbox" :id="id" class="checkbox">
      <label :for="id">
        <div class="tick_mark"></div>
      </label>
    </div>
    <div class="inputText--container">
      <input class="inputText" type="text" value="Нове слово">
    </div>
  </form>
</template>

<script>
export default {
  name: "KeyWord",
  props: {
    id: String,
  },
}
</script>


<style scoped>

.inputText--container {
  position: relative;
  left: 25px;
}

.checkbox--container {
  position: relative;
}

.checkbox {
  display: none;
}

label {
  zoom: 0.2;
  position: absolute;
  top: 50%;
  right: 0;
  left: 0;
  width: 100px;
  height: 100px;
  margin: 0 auto;
  background-color: #f72414;
  transform: translateY(-50%);
  border-radius: 50%;
  box-shadow: 0 7px 10px #ffbeb8;
  cursor: pointer;
  transition: 0.2s ease transform, 0.2s ease background-color,
  0.2s ease box-shadow;
  overflow: hidden;
  z-index: 1;
  border: 2px solid rgba(0, 0, 0, 0.44);
}

label:before {
  content: "";
  position: absolute;
  top: 50%;
  right: 0;
  left: 0;
  width: 70px;
  height: 70px;
  margin: 0 auto;
  background-color: rgba(227, 240, 243, 1);
  transform: translateY(-50%);
  border-radius: 50%;
  box-shadow: inset 0 7px 10px #ffbeb8;
  transition: 0.2s ease width, 0.2s ease height;
  border: 1px solid black;
}

label:hover:before {
  width: 55px;
  height: 55px;
  box-shadow: inset 0 7px 10px #ff9d96;
}

label:active {
  transform: translateY(-50%) scale(0.9);
}

.tick_mark {
  position: absolute;
  top: -1px;
  right: 0;
  left: 0;
  width: 60px;
  height: 60px;
  margin: 0 auto;
  margin-left: 14px;
  transform: rotateZ(-40deg);
}

.tick_mark:before,
.tick_mark:after {
  content: "";
  position: absolute;
  background-color: #fff;
  border-radius: 2px;
  opacity: 0;
  transition: 0.2s ease transform, 0.2s ease opacity;
}

.tick_mark:before {
  left: 0;
  bottom: 0;
  width: 10px;
  height: 30px;
  box-shadow: -2px 0 5px rgba(0, 0, 0, 0.23);
  transform: translateY(-68px);
}

.tick_mark:after {
  left: 0;
  bottom: 0;
  width: 100%;
  height: 10px;
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.23);
  transform: translateX(78px);
}

.checkbox:checked + label {
  background-color: #07d410;
  box-shadow: 0 7px 10px #92ff97;
}

.checkbox:checked + label:before {
  width: 0;
  height: 0;
}

.checkbox:checked + label .tick_mark:before,
.checkbox:checked + label .tick_mark:after {
  transform: translate(0);
  opacity: 1;
}

.inputText {
  width: 80%;
  background: none;
  border: none;
  font-family: 'Roboto', serif;
  font-style: normal;
  font-weight: 520;
  font-size: 16px;
  line-height: 19px;
}

.inputText:hover {
  border-bottom: 2px solid #39AE68;
}

.inputText:focus {
  outline: none;
  background: rgba(255, 255, 255, 0.49);
  border-bottom: 2px solid #39AE68;
}
.container {
    width: 110px;
    height: 19px;
    font-family: 'Roboto', serif;
    font-style: normal;
    font-weight: 500;
    font-size: 12px;
    line-height: 19px;
    display: flex;
    margin: 10px 10px;
  }
</style>