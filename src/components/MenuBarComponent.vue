<template>
  <div id="MainMenubar">
    <span id="MainMenuBarLogo">AL-PM Vue</span>
    <span>|</span>
    <a href="" class="menu-button study">
      <span :style="{ color: pageNum === 1 ? 'black' : 'blue', fontWeight: pageNum === 1 ? 'normal' : 'bold' }">STUDY HOME</span>
    </a>
    <span>|</span>
    <a href="" class="menu-button code"><span>CODE COMMUNITY</span></a>
    <span>|</span>
    <a href="" class="menu-button codegroup"><span>CODE GROUP COMMUNITY</span></a>
    <span>|</span>
    <a href="" class="menu-button mypage"><span>MY PAGE</span></a>
  </div>
</template>

<script>
export default {
  name: 'MenuBarComponent',
  props:{
    pageNum : Number
  }
};
</script>

<style scoped>
#MainMenubar {
  width: 70vw;
  margin-top: 10vh;
  margin-left: 15vw;
  margin-right: 15vw;
  display: grid;
  grid-template-columns: 1fr 0.5fr 1.65fr 0.45fr 2.05fr 0.45fr 2.8fr 0.4fr 1fr;
  justify-items: center;
  font-size: larger;
}

#MainMenuBarLogo  {
  font-weight: bold;
  font-family: 'SUITE-Regular';
}

.menu-button {
  font-family: 'SUITE-Regular';
  background: none;
  border: none;
  cursor: pointer;
  font-size: inherit;
  color: black;
  transition: color 0.3s ease;
  text-decoration : none;
}

.menu-button:hover {
  font-weight: bold;
}

.menu-button.study:hover {
  color: #AFA6FF;
}

.menu-button.code:hover {
  color: #FFB380;
}

.menu-button.codegroup:hover {
  color: #66CC99;
}

.menu-button.mypage:hover {
  color: #FF7F7F;
}

.menu-button.active-study {
  font-weight: bold;
  color: #5C4EFF;
}

.menu-button.active-code {
  font-weight: bold;
  color: #FF6B00;
}

.menu-button.active-codegroup {
  font-weight: bold;
  color: #009418;
}

.menu-button.active-mypage {
  font-weight: bold;
  color: #EF4949;
}

.menu-button-study :active{
  font-weight: bold;
  color: blue;
}
</style>
