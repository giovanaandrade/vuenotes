<template>
  <button @click="OnClick()" :style="{background: color}" class="btn"> {{text}} </button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        text: String,
        color: String,
    },
    methods: {
        OnClick() {
            this.$emit('button-click')
        }
    }

}
</script>

<style>

</style>