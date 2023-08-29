<script setup>

import BaseIcon from "./BaseIcon.vue";
import {computed} from "vue";

const props = defineProps({
    icon: String,
    label: String,
    isActive: Boolean
})

const classes = computed(() => {
    const classes = ["flex", 'items-center', 'px-6', 'py-2', 'text-sm'];

    return props.isActive
        ? [...classes, 'font-medium', 'text-gray-800', "bg-gray-200", "hover:bg-gray-300"]
        : [...classes, 'hover:bg-gray-100']
});

const iconClasses = computed(() => {
    return props.isActive ? 'w-6 h-6 mr-6 text-red-500' : 'w-6 h-6 mr-6';
});


</script>

<template>
    <li>
        <a href="#"
           :class="classes">
            <BaseIcon
                :class="iconClasses"
                :name="icon"
            />
            <span>{{ label }}</span>
        </a>
    </li>
</template>

<style scoped>

</style>