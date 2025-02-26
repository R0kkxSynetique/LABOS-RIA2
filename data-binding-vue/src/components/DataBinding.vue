<script setup>
const props = defineProps({
    name: {
        type: String,
        default: "John Doe",
    },
    items: {
        type: Array,
        default: () => ["Item 1", "Item 2", "Item 3", "Item 4"],
    },
});
</script>

<template>
    <h1>Vue Data Binding</h1>
    <span id="name-container">
        <p>{{ name }}</p>
    </span>
    <ul id="items-container">
        <li v-for="item in items" :key="item">
            {{ item }}
        </li>
    </ul>
</template>
