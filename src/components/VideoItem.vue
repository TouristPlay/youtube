<script setup>


import VideoItemThumbnail from "./VideoItemThumbnail.vue";
import VideoItemInfo from "./VideoItemInfo.vue";

const props = defineProps({
    index: Number
})

</script>

<template>
    <a href="#" class="mb-7 group">
        <VideoItemThumbnail
            :index="index"
        />
        <VideoItemInfo
            :index="index"
        />
    </a>
</template>

<style scoped>

</style>