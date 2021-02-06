<template>
    <div id="book-list">
        <h1 class="title">{{ title }}</h1>
        <ul>
            <li v-for="book in books" :key="book.title">
                <book-item :book=book></book-item>
            </li>
        </ul>
    </div>
</template>

<script>
    import BookItem from './BookItem';

    export default {
        name: 'BookList',
        components: {
            BookItem
        },
        data() {
            return {
                title: 'All Books',
                books: [
                    {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
                    {title: 'American Gods', author: 'Neil Gaiman'},
                    {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
                ]
            };
        }
    }
</script>

<style scoped>
    h1, h2 {
        font-weight: normal;
    }
    ul {
        list-style-type: none;
        padding: 0;
    }
</style>