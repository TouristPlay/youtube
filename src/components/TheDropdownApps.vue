<script setup>

import BaseIcon from "./BaseIcon.vue";
import DropdownAppsListItem from "./DropdownAppsListItem.vue";
</script>

<template>
  <div class="opacity-0 group-hover:opacity-100 absolute top-9 right-0 sm:left-0 bg-white w-60 border border-t-0">
    <section class="py-2 border-b">
      <ul>
        <DropdownAppsListItem
          label="YouTube TV"
        />
      </ul>
    </section>
    <section class="py-2 border-b">
      <ul>
        <li>
          <DropdownAppsListItem
              label="YouTube Music"
          />
        </li>
        <li>
          <DropdownAppsListItem
              label="YouTube Kids"
          />
        </li>
      </ul>
    </section>
    <section class="py-2">
      <ul>
        <li>
          <DropdownAppsListItem
              label="Creator Academy"
          />
        </li>
        <li>
          <DropdownAppsListItem
              label="  YouTube for Artists"
          />
        </li>
      </ul>
    </section>
  </div>
</template>

<style scoped>

</style>