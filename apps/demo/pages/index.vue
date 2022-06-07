<template>
  <div class="center">
    <h2>Demo</h2>
    <div>
      <c-button @click="increment">
        Click me!
      </c-button>
    </div>
    <p>Button clicked {{count}} times!!!</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increment() {
      this.count++;
    }
  }
})
</script>
<style lang="scss" scoped>
h2 {
  font-weight: 400;
}

.center {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
