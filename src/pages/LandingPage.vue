<template>
  <div>
    <button v-for="tab in tabs" :key="tab" @click="selected = tab">
      {{ tab === "CreateGame" ? "Create Game" : "Connect to Game" }}
    </button>

    <component :is="selected"></component>
  </div>
</template>

<script lang="ts">
import ConnectGame from "./ConnectGame.vue";
import CreateGame from "./CreateGame.vue";
export default {
  data: function () {
    return {
      tabs: ["CreateGame", "ConnectGame"],
      selected: "ConnectGame",
    };
  },
  components: {
    CreateGame,
    ConnectGame,
  },
};
</script>
