<template>
  <div class="container">
    <img class="logo" src="../assets/svg/upload.png" alt="img">
    <div class="line"/>
    <img class="logo" src="../assets/svg/size1.png" alt="img">
    <img class="logo" src="../assets/svg/size2.png" alt="img">
    <img class="logo" src="../assets/svg/size3.png" alt="img">
    <div class="line"/>
    <img class="upload" src="../assets/svg/dowload.png" alt="img">
  </div>
</template>

<script>
export default {
  name: "PhotoBar"
}
</script>

<style scoped>

.line {
  box-sizing: border-box;
  width: 3px;
  height: 47px;
  border-left: 1px dashed #000000;
}

.upload {
  height: 35px;
}

.logo {
  height: 45px;
}

.container {
  width: 100%;
  box-sizing: border-box;
  padding: 0 10px;
  height: 67px;
  background-color: #A0A4FD;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

</style>