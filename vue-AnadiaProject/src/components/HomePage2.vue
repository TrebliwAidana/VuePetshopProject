<template>
  <header class="header">
    <a class="header__logo" href="#"> Name </a>
    <div
      class="ham-menu"
      @click="changeVisibility()"
      :class="{ active: burgerVisibility }"
    >
      <span class="ham-menu__item"></span>
      <span class="ham-menu__item"></span>
      <span class="ham-menu__item"></span>
    </div>
    <nav class="header__nav-wrap" :class="{ open: burgerVisibility }">
      <ul class="header__nav-list" @click="burgerVisibility = false">
        <li class="header__nav-item">
          <a class="header__nav-link" href="#">item</a>
        </li>
        <li class="header__nav-item">
          <a class="header__nav-link" href="#">item</a>
        </li>
        <li class="header__nav-item">
          <a class="header__nav-link" href="#">item</a>
        </li>
        <li class="header__nav-item">
          <a class="header__nav-link" href="#">item</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
import { ref } from "vue";

const burgerVisibility = ref(false);

const changeVisibility = () => {
  burgerVisibility.value = !burgerVisibility.value;
};
</script>

<style scoped>
.header {
  display: flex;
  width: 100%;
  background-color: #fff;
  align-items: center;
  position: relative;
  box-sizing: border-box;
  box-shadow: 0px 8px 10px #ccc;
}
@media screen and (max-width: 559px) {
  .header {
    height: 60px;
  }
}
@media screen and (min-width: 560px) and (max-width: 959px) {
  .header {
    height: 70px;
  }
}
@media screen and (min-width: 960px) {
  .header {
    height: 70px;
  }
}
.header__logo {
  display: inline-block;
  height: auto;
  text-decoration: none;
  color: #000;
}
@media screen and (max-width: 559px) {
  .header__logo {
    margin-left: 16px;
    font-size: 18px;
    letter-spacing: 0.07em;
  }
}
@media screen and (min-width: 560px) and (max-width: 959px) {
  .header__logo {
    margin-left: 16px;
    font-size: 24px;
    letter-spacing: 0.05em;
  }
}
@media screen and (min-width: 960px) {
  .header__logo {
    margin-left: 24px;
    font-size: 26px;
    letter-spacing: 0.05em;
  }
}
@media screen and (min-width: 1200px) {
  .header__logo {
    margin-left: 32px;
  }
}
.header__nav-wrap {
  height: 100%;
  width: max-content;
  margin-left: auto;
}
@media screen and (max-width: 959px) {
  .header__nav-wrap {
    position: fixed;
    left: 0;
    top: 0;
    display: none;
    z-index: 10;
    background-color: rgba(0, 0, 0, 0.9);
    width: 100%;
    height: 100%;
  }
}
@media screen and (min-width: 960px) {
  .header__nav-wrap {
    display: inline-block;
    margin-right: 16px;
  }
}
.header__nav-wrap.open {
  display: block;
}
.header__nav-list {
  list-style: none;
  height: 100%;
  margin: 0;
  padding: 0;
}
@media screen and (max-width: 959px) {
  .header__nav-list {
    height: 100%;
    position: relative;
    overflow-x: hidden;
    overflow-y: auto;
    padding-top: 30vh;
  }
}
@media screen and (min-width: 960px) {
  .header__nav-list {
    display: flex;
    align-items: center;
  }
}
.header__nav-item {
  width: max-content;
}
@media screen and (max-width: 559px) {
  .header__nav-item {
    display: block;
    margin: 0 auto;
    margin-bottom: 32px;
    text-align: center;
  }
}
@media screen and (min-width: 560px) and (max-width: 959px) {
  .header__nav-item {
    display: block;
    margin: 0 auto;
    margin-bottom: 40px;
    text-align: center;
  }
}
@media screen and (min-width: 960px) {
  .header__nav-item {
    display: inline-block;
    margin-right: 24px;
  }
}
@media screen and (min-width: 1200px) {
  .header__nav-item {
    margin-right: 40px;
  }
}
.header__nav-link {
  position: relative;
  display: inline-block;
  text-decoration: none;
  letter-spacing: 0.15em;
  color: #1a1c1a;
}
@media screen and (max-width: 959px) {
  .header__nav-link {
    font-size: 21px;
    color: #fff;
  }
}
@media screen and (min-width: 960px) {
  .header__nav-link {
    font-size: 18px;
  }
}
@media screen and (min-width: 1200px) {
  .header__nav-link {
    font-size: 20px;
  }
}
.header__nav-link::after {
  position: absolute;
  bottom: -4px;
  left: 0;
  content: "";
  width: 100%;
  height: 2px;
  transform: scale(0, 1);
  transform-origin: center top;
  transition-duration: 0.25s;
}
@media screen and (max-width: 959px) {
  .header__nav-link::after {
    background-color: #fff;
  }
}
@media screen and (min-width: 960px) {
  .header__nav-link::after {
    background-color: #1a1c1a;
  }
}
.header__nav-link:hover::after {
  transform: scale(1, 1);
}

@media screen and (max-width: 959px) {
  .ham-menu {
    display: inline-block;
    box-sizing: border-box;
    margin-left: auto;
    margin-right: 16px;
    transition: all 0.3s;
    z-index: 20;
    position: relative;
    width: 40px;
    height: 40px;
    background-color: transparent;
    display: flex;
    justify-content: center;
    border-radius: 5px;
    border: 2px solid #000;
    cursor: pointer;
  }
}
@media screen and (min-width: 960px) {
  .ham-menu {
    display: none;
  }
}
@media screen and (max-width: 959px) {
  .ham-menu__item {
    display: inline-block;
    box-sizing: border-box;
    transition: all 0.3s;
    position: absolute;
    width: 30px;
    height: 4px;
    background-color: #000;
    border-radius: 5px;
  }
}
.ham-menu__item:nth-of-type(1) {
  top: 8px;
}
.ham-menu__item:nth-of-type(2) {
  top: 16px;
}
.ham-menu__item:nth-of-type(3) {
  bottom: 8px;
}
.ham-menu.active {
  border: none;
}
.ham-menu.active .ham-menu__item:nth-of-type(1) {
  -moz-transform: translateY(10px) rotate(-45deg);
  -webkit-transform: translateY(10px) rotate(-45deg);
  transform: translateY(10px) rotate(-45deg);
  background-color: #fff;
}
.ham-menu.active .ham-menu__item:nth-of-type(2) {
  transition-duration: 0s;
  opacity: 0;
}
.ham-menu.active .ham-menu__item:nth-of-type(3) {
  -moz-transform: translateY(-10px) rotate(45deg);
  -webkit-transform: translateY(-10px) rotate(45deg);
  transform: translateY(-10px) rotate(45deg);
  background-color: #fff;
}
</style>
