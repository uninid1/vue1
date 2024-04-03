<template>
  <div id="app">
    <h1>Компонент профиля пользователя</h1>
    <user-profile :user="user"></user-profile>
  </div>
</template>

<script>
import UserProfile from "./components/UserProfile.vue";

export default {
  name: "App",
  components: {
    UserProfile
  },
  data() {
    return {
      user: {
        name: "uninid1",
        avatarUrl: "https://avatar-url",
        
        bio: "Пользователь",
        followers: 1,
        following: 0
      }
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>