<script type="module">
import { createApp } from "vue";

export default createApp({
  data() {
    return {
      awesome: true,
    };
  },
  methods: {
    toggle() {
      this.awesome = !this.awesome;
    },
  },
}).mount("#app");
</script>

<div id="app">
  <button @click="toggle">toggle</button>
  <h1 v-if="awesome">Vue is awesome!</h1>
  <h1 v-else>Oh no 😢</h1>
</div>
