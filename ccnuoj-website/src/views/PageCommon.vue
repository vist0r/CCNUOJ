<template>

<!-- 根组件（除了APP.VUE) -->
<el-container>

  <!-- <nav-menu/> -->

  <el-main>
    <nav-menu/>
    <p class="title">CCNU Online Judge</p>
    <div class="content">
      <slot></slot>
    </div>
  </el-main>

</el-container>

</template>

<script>

import NavMenu from '../components/NavMenu';

export default {
  name: 'PageCommon',
  data() {
    return {
    };
  },
  components: {
    NavMenu,
  },
};

</script>

<style lang="css" scoped>
.el-main {
  padding: 0;
}

.title{
  padding: 20px 0 10px;
  text-align: center;
  font-size: 40%;
}

.content{
  padding: 10px 20px;
}

</style>
