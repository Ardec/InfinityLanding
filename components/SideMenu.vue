<template>
  <div class="overlay-menu" v-if="menuVisible">
    <div class="header-container">
      <div class="button">
        <div class="menu-icon-container" @click="toggleMenu"><Icon class="icon" name="material-symbols:close" /></div>
        </div>
      <div class="title">InfinityUp</div>
      <div class="sub-title">Najszybciej rozwijający się przewoźnik taxi we Wrocławiu</div>
    </div>
    <div class="navigation">
        <nav>
       <ul>
          <li><NuxtLink class="menu-item active" to="/" @click="toggleMenu">Home</NuxtLink></li>
        </ul>
    </nav>
    </div>
    <div class="partners">
      <div class="description">
      </div>
      <div class="section">
    </div>
    </div>
  </div>
</template>

<script setup>
import { useGlobalState } from '~/composables/useGlobalState';
const { menuVisible, toggleMenu } = useGlobalState();
const baseUrl = useBaseUrl();

// Zmienna kontrolująca widoczność menu
const isVisible = ref(true);

// Tutaj możesz dodać logikę otwierania/zamykania menu
</script>

<style lang="scss" scoped>
*{
  color:$text-primary;
}
.menu-icon-container{
  font-size:28px;
}
.menu-icon-container:hover{
 cursor:pointer;
}

.overlay-menu {
  position: fixed;
  top: 0;
  left: 0;
  width: 320px;
  height: 100%;
  background: $primary;
  box-shadow: 0px 0px 20px 2px $primary(0, 0, 0, 0.25);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  z-index: 100;
}

// .overlay-menu::before {
//   content: '';
//   position: absolute;
//   top: 0;
//   left: 0;
//   width: 100%;
//   height: 100%;
//   background-size: cover;
//   z-index: -1;
//   opacity: 0.5; /* Dostosuj wartość dla odpowiedniego poziomu przyciemnienia */
// }

.header-container{
  margin:8px 24px;
  display:flex;
  flex-direction: column;
  }

.title{
margin-top:24px;
font-size: 34px;
font-style: normal;
font-weight: 700;
line-height: 39px; /* 114.706% */
  }
.description {
  font-family: Inter;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 29px; /* 161.111% */
  align-self: start;
}
.button{
  align-self: flex-end;
  cursor:pointer;
}
.menu-item {
  color:black;
  display: flex;
  align-items: center;
  margin-bottom:2px;
  padding: 12px 0px 12px 16px;
  border-radius: 6px;
  font-size:16px;
  line-height: 24px;
}
.menu-item:hover {
  cursor:pointer;
  opacity:0.6;

}
.active{
color:$primary;
background: var(--Gray-050, #F7F8F9); 
}
.navigation{
  margin-top:200px;
  padding: 0px 20px;
}
.partners{
  padding:0px 20px;
}

nav ul {
  list-style: none;
  padding: 0;
}
nav ul li a {
  text-decoration: none;
}
.sections{
    padding:0px 10px;
}
.section-title {
  justify-content: space-between;
  display: flex;
  flex-direction: row;
  color: #000;
  font-family: Poppins;
  font-size: 28px;
  font-style: normal;
  font-weight: 700;
  line-height: 32px; /* 114.286% */
  margin-top: 8px;
}
.item {
  // height: 100px;
  width: 100px;
  // background-color: black;
  border-radius: 4px;
}
.image {
  border-radius: 4px;
}
img {
  width: 100px;
  height: 100px;
  border-radius: 4px;
}
.section-box {
  // background-color: red;
  padding: 8px 0px;
  display: flex;
  flex-direction: row;
  gap: 12px;
  overflow-x: auto; /* Enable horizontal scrolling */
  overflow-y: hidden; /* Hide vertical scrollbar */
  scrollbar-width: thin; /* Można ustawić 'auto', 'thin' lub 'none' */
  scrollbar-color: $accent transparent; /* Kolor suwaka i tła (ścieżki) */
}
/* Stylizowanie paska przewijania dla przeglądarek WebKit */
.section-box::-webkit-scrollbar {
  height: 8px; /* Grubość paska przewijania */
}

.section-box::-webkit-scrollbar-track {
  background: transparent; /* Kolor tła ścieżki paska przewijania */
}

.section-box::-webkit-scrollbar-thumb {
  background: orange; /* Kolor suwaka paska przewijania */
  border-radius: 2px; /* Zaokrąglenie krawędzi suwaka */
  min-height: 20px; /* Minimalna długość suwaka */
}
</style>
