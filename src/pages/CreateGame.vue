<template>
  <div>
    <h2>Create a New Game</h2>
    <form>
      <label>Enter your games's ID</label>
      <input type="text" v-model="roomId" />
      <label>Enter your player name</label>
      <input v-model="playerName" type="text" />
      <button @click.prevent="createGame">Create game</button>
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
    createGame() {},
  },
};
</script>

<style scoped>

</style>
