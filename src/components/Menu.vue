<template>
  <el-menu :default-active="activeLink" mode="horizontal" :router="true">
    <el-menu-item index="/">
      <i class="el-icon-menu"></i>
      <span>Home</span>
    </el-menu-item>
    <el-menu-item index="/istruzioni">
      <i class="el-icon-cloudy"></i>
      <span>Istruzioni</span>
    </el-menu-item>
  </el-menu>
</template>

<script>
import _ from "lodash";

export default {
  mounted: function() {
    let match = _.chain(this.$route.matched)
      .sortBy(n => n.path.length)
      .last()
      .value();
    this.activeLink = match.path;
  },
  data() {
    return {
      activeLink: null
    };
  }
};
</script>
