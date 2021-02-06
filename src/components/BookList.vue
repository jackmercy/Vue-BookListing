<template>
    <div id="book-list">
        <h1 class="title">{{ title }}}</h1>
    </div>
</template>

<script>
    export default {
        name: 'BookList',
        data() {
            return {
                title: 'All Books'
            };
        }
    }
</script>

<style scoped>
    h1, h2 {
        font-weight: normal;
    }
</style>