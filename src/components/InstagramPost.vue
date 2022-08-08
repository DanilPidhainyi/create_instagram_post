<!--it`s automatic instagram make post-->
<template>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Nunito&display=swap" rel="stylesheet">
  <div class="container">
    <header class="header">
      <figure class="ava"/>
      <strong>user_name</strong>
      <img class="ico ico--right" src='../assets/svg/settings.jpg'/>
    </header>
    <body class="body">
      <img  src="../assets/test.jpg" />
      <ul class="ico__container">
        <li><img class="ico" src='../assets/svg/like.jpg'/></li>
        <li><img class="ico" src='../assets/svg/coment.jpg'/></li>
        <li><img class="ico" src='../assets/svg/spread.jpg'/></li>
        <li><img class="ico ico--right" src='../assets/svg/save.jpg'/></li>
      </ul>
    </body>
    <footer>
      <p>
        Уподобали <strong>user_name</strong> і <strong>ще</strong>
      </p>
      <p>
        <strong>user_name</strong> Напиши слово 3 раза в комментариях, чтобы лучше запомнить! 📖
        <br/><br/>
        Хотите ускорить процесс изучения Английского ?<br/>
        1. Для лучшего запоминания слова напишите его 3 раза в комментариях. ✍️
        <br/><br/>
        2. Расскажите о моем блоге друзьям, родным и коллегам по работе. Учить Английский вместе намного интереснее и веселее!!!! 🗣
        <br/><br/>
        3. Включите уведомления о новых публикациях, чтобы не пропускать новые слова! Сделать это можно перейдя в мой профиль и в правом верхнем углу нажав на три точки. Далее необходимо нажать "включить уведомления о публикациях". Готово, больше вы не пропустите новых слов! 🔊
        <br/><br/>
      </p>
      <p class="lick">
         #английскийязык #английский #английскийонлайн #английскийдляначинающих #английскийдлявзрослых #английскийдлядетей #учительанглийского #репетиторанглийского #репетитор #репетиторонлайн #englishonline #english #englishteacher #englishlearning #teacherblog #teacherblog
      </p>
      <p class="grey">
        Переглянути всі коментарі: 236
      </p>
      <p class="grey f12_8">
        1 ГОДИНУ ТОМУ
      </p>
    </footer>
    <hr/>
    <section class="comments__container">
      <img class="comments--ico" src="../assets/svg/face.png" alt="голова">
      <p class="grey">Додайте коментар...</p>
      <p class="comments--send"><strong>Опублікувати</strong></p>
    </section>
  </div>
</template>

<script>

export default {
  name: "InstagramPost",

  components: {
  }
}
</script>

<style scoped>

@font-face {
font-family: "Inheritance";
src: url("../assets/fonts/Inheritance.ttf") format("truetype");
  font-style: normal;
  font-weight: normal;
}

.f12_8{
  font-size: 10px;
}

.lick {
  color: rgb(37, 68, 93);
}

.grey {
  margin: 8px 0 8px 0;
  color: rgb(0, 0, 0, .6);
}
.comments--send {
  position: absolute;
  right: 12px;
  color: rgb(71, 65, 250, .6);
}

.comments--ico {
  width: 24px;
  height: 24px;
  margin: 0 16px 0 12px;
}

* {
  --border-with: 1px;
  --border-color: rgba(23, 22, 22, 0.4);
}

.comments__container {
  max-width: 100%;
  height: 36px;
  padding: 0 0 4px 0;
  display: flex;
  align-items: center;
  position: relative;
}

hr {
  border: none;
  height: 1px;
  background-color: var(--border-color);
}

footer {
  max-width: 100%;
  height: max-content;
  padding: 0 12px 12px 12px;

}

p {
  margin: 0 8px 0 0;
  padding: 0;
}

body {
  background-color: white;
}

img {
  width: 100%;
  height: auto;
}

.container {
  width: 470px;
  height: max-content;
  border-radius: 8px;
  background-color: white;
  /*overflow: hidden;*/
  border: solid var(--border-color) var(--border-with);
  font-family: 'Nunito', sans-serif;
  font-size: 14px;
}

.header {
  width: 100%;
  height: 56px;
  display: flex;
  align-items: center;
  position: relative;
}

header .ico {
  width: 20px;
  height: 20px;
  object-fit:cover;
  margin: 6px 12px 6px 12px;
}



header .ava {
  margin: 0 10px 0 12px;
  padding: 0;
  width: 32px;
  height: 32px;
  border-radius: 50%;
  background-color: #ec0049;

}

.ico__container {
  margin: 0;
  padding: 4px;
  list-style: none;
  max-width: 100%;
  height: 46px;
  display: flex;
  align-items: center;
  flex-wrap: nowrap;
  position: relative;
}

li{
  margin: 0;
  padding: 0;
}

.ico {
  width: 24px;
  height: 24px;
  object-fit:cover;
  margin: 6px 8px 6px 8px;
}

.ico--right {
  position: absolute;
  right: 0;
  top: 50%;
  transform: translateY(-20px);
}
</style>