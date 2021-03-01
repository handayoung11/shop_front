<template>
  <div>
    <b-navbar type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item href="/">Home</b-nav-item>

        <!-- Navbar dropdowns -->
        <!--        <b-nav-item-dropdown text="Lang" right>-->
        <!--          <b-dropdown-item href="#">EN</b-dropdown-item>-->
        <!--          <b-dropdown-item href="#">ES</b-dropdown-item>-->
        <!--          <b-dropdown-item href="#">RU</b-dropdown-item>-->
        <!--          <b-dropdown-item href="#">FA</b-dropdown-item>-->
        <!--        </b-nav-item-dropdown>-->

        <b-nav-item-dropdown text="User" right>
          <b-dropdown-item v-b-modal.login-modal href="#"
            >Sign in</b-dropdown-item
          >
          <b-dropdown-item href="#">Sign up</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-navbar>
    <login />
  </div>
</template>

<script>
import login from '@/layouts/login'
export default {
  name: 'Header',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    login,
  },
}
</script>

<!--<style scoped></style>-->
