<script setup>
import DataBinding from "@/components/DataBinding.vue";

const items = ["Item 1", "Item 2", "Item 3", "Item 4"]
const name = "John Doe"

</script>

<template>
    <DataBinding :name="name" :items='items'/>
</template>
