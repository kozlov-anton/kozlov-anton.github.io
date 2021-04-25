<template>
    <div class="posts">
        <ul>
            <PostItem
                v-for="todo of todos" :key="todo.id"
                v-bind:todo="todo"
            />
        </ul>
    </div>
</template>

<script>
    import PostItem from './PostItem'
    export default {
        props: ['todos'],
        components: {
            PostItem
        }
    }
</script>