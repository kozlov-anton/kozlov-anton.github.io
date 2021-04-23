<template>
    <div class="main">
        <Posts/>
    </div>
</template>

<script>
    import Posts from './Posts'

    export default {
        name: 'Content',
        components: {
            Posts
        }
    }
</script>

<style scoped>
    .main {
        border: 1px solid #ccc;
        padding: 15px;
        margin-top: 10px;
    }
</style>