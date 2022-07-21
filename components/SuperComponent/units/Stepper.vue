<template>
  <div>
    <h1>I`m a super puper Stepper</h1>
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { defineComponent } from '@nuxtjs/composition-api'

export default defineComponent({
  name: 'SuperDuperStepper',
})
</script>
