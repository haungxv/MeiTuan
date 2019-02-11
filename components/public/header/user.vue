<template>
  <div class="m-user">
    <template v-if="user">
      欢迎您，<sapn class="username">{{user}}</sapn>
      [<nuxt-link to="/exit">退出</nuxt-link>]
    </template>
    <template v-else>
      <nuxt-link to="/login" class="login">立即登陆</nuxt-link>
      <nuxt-link to="/register" class="register">注册</nuxt-link>
    </template>
  </div>
</template>

<script>
  export default {
    name: "user",
    data() {
      return {
        user: ''
      }
    }
  }
</script>

<style scoped>

</style>
