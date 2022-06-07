<template>
    <button v-bind="$attrs" class="my-button" @click="$emit('click')">
        <slot />
    </button>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'CButton',
    props: {
        label: String
    }
})
</script>
<style lang="scss" scoped>
.my-button {
    padding: 5px 8px;
    border: 1px solid grey;
    border-radius: 4px;
    background: blue;
    color: white;
    &:hover {
        background: darkblue;
    }
}
</style>