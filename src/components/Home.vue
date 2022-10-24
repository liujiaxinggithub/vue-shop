<template>
  <di>
    <el-button type="info" @click="logout">退出</el-button>
  </di>
</template>

<script>
export default {
  name: 'MyHome',
  methods: {
    logout() {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>
</style>
