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
                title: 'All books'
            };
        }
    }
</script>

<style scoped>
    .title {
        font-weight: normal;
    }
</style>