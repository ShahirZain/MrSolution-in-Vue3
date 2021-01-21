<template>
  <div id="nav"></div>
  <navBar/>
  <router-view />
</template>
<script>
import navBar from './components/landingPage/nav/nav'
export default {
  components: {navBar}
}
</script>
<style></style>
