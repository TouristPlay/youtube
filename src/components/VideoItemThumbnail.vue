<script setup>

    import BaseIcon from "./BaseIcon.vue";

    const props = defineProps({
        index: Number
    })

</script>

<template>
    <div class="relative">
        <img src="../assets/images/video/video.jpg">
        <span
            class="opacity-0 group-hover:opacity-100 bg-opacity-60 absolute top-0 right-0 bg-black text-white rounded-sm m-1 p-1">
            <BaseIcon
                name="clock"
                class="w-5 h-5"
            />
          </span>
        <span
            class="opacity-0 group-hover:opacity-100 bg-opacity-60 absolute top-8 right-0 bg-black text-white rounded-sm m-1 p-1">
            <BaseIcon
                name="menuAlt3"
                class="w-5 h-5"
            />
          </span>
        <span
            class="opacity-100 group-hover:opacity-0 duration-500 absolute bottom-0 right-0 bg-black text-white rounded-sm m-1 p-1 text-xs font-semibold">6:35</span>
    </div>
</template>

<style scoped>

</style>