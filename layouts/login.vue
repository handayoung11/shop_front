<template>
  <div>
    <b-modal
      id="login-modal"
      title="Login"
      ok-only
      ok-title="Cancel"
      ok-variant="secondary"
    >
      <el-input v-model="loginId" placeholder="Input your ID"></el-input>
      <el-input
        v-model="loginPW"
        placeholder="Input your password"
        style="margin-top: 15px"
      ></el-input>
      <el-button type="primary" round>Sign in</el-button>
    </b-modal>
  </div>
</template>

<script>
export default {
  name: 'Login',
  data() {
    return {
      loginId: '',
      loginPW: '',
    }
  },
}
</script>

<style>
.el-input__inner {
  width: 100%;
}
</style>
