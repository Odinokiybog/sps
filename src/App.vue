<template>
  <div class="navigation">
    <div class="logotype">
      <img src="./assets/Logotype.svg" alt="logotype">
    </div>
    <nav>
      <router-link to="/auth">Авторизация</router-link> |
      <router-link to="/registration">Регистрация</router-link>
      <router-link to="/">Регистрация</router-link> 
      <router-link to="/">Мероприятия</router-link> 
      <router-link to="/">Партнерам</router-link>
      <router-link to="/">Контакты</router-link>  
    </nav>
    <router-view/>
  </div>
  
</template>

<style>
* {
  margin: 0;
  padding: 0;
}
@font-face {
  font-family: 'JetBrains Mono';
  src: url('./fonts/JetBrainsMonoNL-Regular.ttf');
}
#app {
  font-family: 'JetBrains Mono';
  background-color: #1B1C21;
}
.navigation {
  display: flex;
  flex-direction: row;
  height: 80vh;
}
nav {
  padding: 0px;
}

nav a {
  font-weight: bold;
  color: #D9D9D9;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: blue;
}
</style>
