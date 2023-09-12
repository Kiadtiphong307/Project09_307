<script setup>
import { ref } from "vue";
defineProps(['title'])

const counter = ref(0);

function plus(title) {
    switch(title) {
        case "Like_1":
            counter.value += 10;
            break;
        case "Love_1":
            counter.value += 500;
            break;
        case "Drop_1":
            counter.value -= 800;
            break;
    }
}
</script>

<template>
    <div>
        <button @mouseover="plus(title)">{{ title }} {{counter}}</button>
    </div>

 
</template>

<style>
</style>