<template>
  <div class="w-auto p-3 bg-red-200 rounded-lg" :class="type">
      <slot></slot>
  </div>
</template>

<script>
export default {
  props:{
    type:String
  }
}
</script>

<style>

</style>