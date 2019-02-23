<template>
  <div id="page">
    <TheHeader/>
    <TheFooter/>
  </div>
  
</template>

<script>
import TheHeader from '@/components/layouts/TheHeader'
import TheFooter from '@/components/layouts/TheFooter'
  export default {
    name: 'App',
    components: {
      TheHeader,
      TheFooter
    }
  }
</script>

<style lang='scss'>
  $backgroundColor: #cccccc;
  $itembackground: blue;
  body{
    background: $backgroundColor;
  }


// 下面这里主要是引入外面的sass、字体文件、bootstrap框架等

// @import "~bootstrap-sass/assets/stylesheets/_bootstrap";
// @import "~font-awesome/scss/font-awesome";
// @import "./styles/main";
// @import "./styles/extra";
</style>
