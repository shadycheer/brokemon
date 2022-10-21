<style scoped lang="postcss">
.bm-button {

}
</style>

<template>
  <div class="bm-button" >
    <slot/>
  </div>
</template>

<script lang="ts" setup>

import {ButtonProps} from './types'

interface Button extends ButtonProps {

}

const props = withDefaults(defineProps<Button>(), {
  disabled: false,
  loading: false,
  shape: 'default',
  type: 'primary',
  size: 'normal',
})

const onChange = (e) => {
  console.log(e.target.value)
}

const {} = props

</script>