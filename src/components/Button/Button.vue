<style scoped>

</style>

<template>
  <button><slot/></button>
</template>

<script lang="ts" setup>
import {reactive, ref} from 'vue'

const a = ref(0)

</script>