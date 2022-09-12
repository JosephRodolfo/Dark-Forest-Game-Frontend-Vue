<template>
  <div>
    <h2>Connect to Game</h2>
    <form>
      <label>Enter your room ID</label>
      <input type="text" v-model="roomId" />
      <label>Enter your player name</label>
      <input v-model="playerName" type="text" />
      <button @click.prevent="signIn">Connect</button>
    </form>
  </div>
</template>
<script lang="ts">
export default {
  data() {
    return {
      roomId: "",
      playerName: "",
    };
  },
  methods: {
    signIn() {},
  },
};
</script>

<style scoped>

</style>
