<template>
    <p @click="callEmit">Click me!!!!!  Do it now!!!!</p>
</template>

<script>
export default {
    name: 'Clickydoo',
    methods: {
        callEmit(e) {
            console.log(e.target);
            this.$emit("goTime", e.target.innerText);
        }
    },
}
</script>

<style>

</style>