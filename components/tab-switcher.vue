<template>
  <img :src="index == activeTab ? activeImage : inactiveImage" />
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    index: {
      type: Number,
      default: 0,
      required: true,
    },
    activeTab: {
      type: Number,
      default: 0,
      required: true,
    },
    activeImage: {
      type: String,
      required: true,
    },
    inactiveImage: {
      type: String,
      required: true,
    },
  },
})
</script>
