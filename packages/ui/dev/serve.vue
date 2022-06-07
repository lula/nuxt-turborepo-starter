<script lang="ts">
import Vue from 'vue';
// Uncomment import and local "components" registration if library is not registered globally.
// import { ClubchainWebUiSample } from '@/entry.esm';

export default Vue.extend({
  name: 'ServeDev',
  // components: {
  //  ClubchainWebUiSample,
  // }
});
</script>

<template>
  <div id="app">
    <clubchain-web-ui-sample />
  </div>
</template>
