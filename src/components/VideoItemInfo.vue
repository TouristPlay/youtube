<script setup>

import BaseIcon from "./BaseIcon.vue";

const props = defineProps({
    index: Number
})


</script>

<template>
    <div class="flex items-start mt-3">
        <img src="../assets/images/channel/channel.jpg" class="mr-3 rounded-full w-9 h-9" alt="">
        <div class="text-sm">
            <span class="font-semibold text-gray-800">Video title {{index}}</span>
            <div class="mt-1 flex items-center">
                <span>Channel name</span>
                <BaseIcon
                    name="checkCircle"
                    class="w-3.5 h-3.5 ml-1"
                />
            </div>
            <div>
                {{index}}K views &middot; {{index}} day ago
            </div>
        </div>
        <button
            class="-mt-1 ml-auto p-1 opacity-0 group-hover:opacity-100 text-gray-500 hover:text-gray-700 focus:outline-none">
            <BaseIcon
                name="dostVertical"
            />
        </button>
    </div>
</template>

<style scoped>

</style>