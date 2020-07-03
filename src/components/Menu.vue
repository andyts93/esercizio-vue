<template>
  <el-menu
    :default-active="activeLink"
    mode="horizontal"
    :router="true"
    background-color="#545c64"
    text-color="#fff"
    active-text-color="#ffd04b"
  >
    <el-menu-item index="/">
      <i class="el-icon-menu"></i>
      <span>Home</span>
    </el-menu-item>
    <el-menu-item index="/istruzioni">
      <i class="el-icon-info"></i>
      <span>Istruzioni</span>
    </el-menu-item>
  </el-menu>
</template>

<script>
export default {
  mounted: function() {
    this.activeLink = this.$route.path;
  },
  watch: {
    $route(newVal) {
      this.activeLink = newVal.path;
    }
  },
  data() {
    return {
      activeLink: null
    };
  }
};
</script>
