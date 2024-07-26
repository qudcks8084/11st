<template>
  <div class="menu">
    <ul class="menubar">
      <li v-for="(eachmenu, index) in menubar1" :key="index"><a href="#">{{eachmenu}}</a></li>
      <li><span>|</span></li>
      <li v-for="(eachmenu, index) in menubar2" :key="index"><a href="#">{{eachmenu}}</a></li>
      <li><span>|</span></li>
      <li><a href="#">아마존</a></li>
    </ul>
    <ul class="menubar">
      <li><a href="#">로그인</a></li>
      <span>바로가기</span>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MenuBarComponent',
  data() {
    return {
      menubar1: ['베스트', '쇼킹딜', '슈팅배송', '쿠폰/기획전'],
      menubar2: ['신선식품', '장보기', '9900원샵', '리퍼블리', 'T공식대리점'],
    };
  },
};
</script>

<style scoped>
.menu {
  width: 1200px;
  display: flex;
  justify-content: center;
  text-align: center;
  background: white;
  border-color: gray;
  border-radius: 5px;
  flex-shrink: 0;
}

.menubar {
  list-style-type: none;
  display: flex;
  align-items: center;
  padding: 0;
  margin: 0;
}

.menubar li {
  margin-right: 10px;
}

.menubar li a {
  color: black;
  text-decoration: none;
  font-weight: 600;
}

</style>
