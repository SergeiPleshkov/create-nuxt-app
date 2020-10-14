<template>
  <div
    style="display: flex; flex-flow: column;"
  >
    <n-link :to="to" :href="href">
      value taken from prop (not set)
    </n-link>
    <n-link :to="to" :href="undefined">
      undefined
    </n-link>
    <n-link :to="to">
      no :href passed to n-link
    </n-link>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: ['to', 'href']
})
</script>
