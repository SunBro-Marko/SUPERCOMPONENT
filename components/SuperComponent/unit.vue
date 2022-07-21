<template>
  <div v-if="toggle">
    <h1>С детьми</h1>
    <component :is="`SuperComponentUnits${name}`">
      <component
        v-for="_item in 10"
        :key="Math.random()"
        :is="`SuperComponentUnits${name}`"
      ></component>
    </component>
  </div>
  <div v-else>
    <h1>Безе детей</h1>
    <component :is="`SuperComponentUnits${name}`"></component>
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api'

export default defineComponent({
  name: 'SuperDuperInit',
  props: {
    name: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      toggle: true,
    }
  },
})
</script>
