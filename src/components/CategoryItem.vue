<script setup>

  import {computed} from "vue";

  const props = defineProps({
    category: String,
    isActive: Boolean
  })

  const classes = computed(() => {
    const classes = [
      'px-3', 'py-1', 'transition', 'rounded-full', 'border',
    ];


    return props.isActive
        ? [...classes, 'bg-gray-600', 'border-gray-700',  'hover:bg-gray-500', 'text-white']
        : [...classes, 'bg-gray-100', 'border-gray-300',  'hover:bg-gray-200',]
  });


</script>

<template>
  <a href="#"
     :class="classes">
    {{ category }}
  </a>
</template>

<style scoped>

</style>