<template>
  <div>
    <h1>I`m a super puper Component</h1>
    <SuperComponentUnit name="Stepper" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api'

export default defineComponent({
  name: 'SuperDuperComponent',
})
</script>
