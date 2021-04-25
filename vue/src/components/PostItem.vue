<template>
    <li>
        <input v-bind:id="'checkTodo-' + todo.id" type="checkbox" v-on:change="todo.completed = !todo.completed"/>
        <label v-bind:for="'checkTodo-' + todo.id">
            <span>{{todo.title}}</span>
        </label>
    </li>
</template>

<script>
    export default {
        name: 'PostsItem',
        props: {
            todo: {
                type: Object,
                required: true
            }
        }
    }
</script>