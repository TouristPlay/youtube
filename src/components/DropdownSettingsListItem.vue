<script setup>

import BaseIcon from "./BaseIcon.vue";

const props = defineProps({
    label: String,
    icon: String,
    withSubMenu: Boolean
})

</script>

<template>
    <li>
        <a href="#" class="flex items-center px-4 py-2 text-sm hover:bg-gray-100">
            <BaseIcon
                v-if="icon"
                :name="icon"
                class="w-6 h-6 mr-3 text-gray-400"
            />
            <span>{{ label }}</span>
            <BaseIcon
                v-if="withSubMenu"
                name="chevronRight"
                class="w-5 h-5 text-gray-400 ml-auto"
            />
        </a>
    </li>
</template>

<style scoped>

</style>