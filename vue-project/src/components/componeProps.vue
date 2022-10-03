<template>
    <div>
        <h2>{{name}}</h2>
        <h3>{{age}}</h3>
        <h4>{{birthplace}}</h4>
        <h5>{{currentLocation}}</h5>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

defineProps({
    name: {
        type: String,
        default: "A nose",
    },
    age: {
        type: String,
        default: "400",
    },
    birthplace: {
        type: String,
        default: "Colombia Medellin",
    },
    currentLocation: {
        type: String,
        default: "La cova del llop",
    },
});
</script>

<style scoped>

</style>