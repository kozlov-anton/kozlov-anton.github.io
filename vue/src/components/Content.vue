<template>
    <div class="main">
        <img v-if="isImg" src="../assets/logo.png" alt="" width="100" height="100">
        <Posts v-bind:todos="todos"/>
        <button v-on:click="AddToCart">Add to Cart {{cart}}</button>
    </div>
</template>

<script>
    import Posts from './Posts'

    export default {
        name: 'Content',
        props: ['todos'],
        components: {
            Posts
        },
        data() {
            return {
                isImg: true,
                cart: 0
            }
        },
        methods: {
            AddToCart: function () {
                this.cart += 1
            }
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