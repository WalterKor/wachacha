<template>
  <div class="menu">
    
    <div class="leftMenu">
      <a v-for="menu in menu" :key="menu">{{menu}}</a>
    </div>
  
    <div class="rightMenu">
      <a v-for="rightMenu in rightMenu" :key="rightMenu">{{rightMenu}}</a>
    </div>
    
  </div>  

</template>

<script>


export default {
  name: 'App',
  // 데이터 임시저장
  data() {
    return {
      
      menu : ['홈', '탐색하기', '평가하기'],
      rightMenu : ['검색', '보고싶어요', '프로필']

    }
  },

  components: {
    
  }
}
</script>


<style>

</style>
