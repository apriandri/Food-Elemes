<template>
  <section class="mb-14">
      <div class="my-2 mb-9">
          <p class="font-semibold text-2xl md:text-4xl">{{ mainTitle }}</p>
          <p style= "color: #8BAC3E" class="text-lg md:text-3xl font-semibold">{{ secondTitle }}</p>
      </div>
      <div class="my-2">
          <slot name="mainMenus"></slot>
      </div>
  </section>
</template>
s
<script>
export default {
    name: 'VSection',
    props: {
        mainTitle: {
            require: true,
            type: String,
            default: 'Browser Our Menus'
        },
        secondTitle: {
            type:String,
            default: 'Receipt'
        }
    }
}
</script>

<style>

</style>