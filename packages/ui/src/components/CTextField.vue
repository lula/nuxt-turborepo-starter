<template>
    <div>
        <div>{{test}}</div>
        <input v-model="text" type="text" @input="$emit('input', text)" class="test">
        <div>ciaaaao</div>
        <p>{{name}}</p>
    </div>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'CTextField',
    props: {
        /** model */
        value: String,

        /** test attribute */
        name: String
    },
    data() {
        return {
            text: (this.value || '') + '___pooo'
        }
    }
})
</script>

<style lang="scss" scoped>
.test {
    border: 1px solid grey;

    &:hover {
        border: 1px solid red;
    }
}
</style>