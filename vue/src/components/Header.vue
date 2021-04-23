<template>
    <header>Header of {{ msg }}</header>
</template>

<script>
    export default {
        name: 'Header',
        props: {
            msg: String
        }
    }
</script>

<style scoped>
    header {
        padding: 15px;
        background: #accba6;
        font-weight: bold;
    }
</style>