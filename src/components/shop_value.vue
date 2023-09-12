<script setup>
const list = defineProps({
    name:String,
    price:Number,
    image:String,
})


</script>

<template>
    <div>
        name = {{ list.name }}
        price = {{ list.price }}
        image = {{ list.image }}
    </div>
</template>