<template>
  <div class="user-profile">
    <h2>{{ user.name }}</h2>
    <img :src="user.avatarUrl" alt="User Avatar">
    <p>{{ user.bio }}</p>
    <p>Followers: {{ user.followers }}</p>
    <p>Following: {{ user.following }}</p>
  </div>
</template>

<script>
export default {
  props: {
    user: {
      type: Object,
      required: true
    }
  }
};
</script>

<style>
.user-profile {
  text-align: center;
}

img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
</style>