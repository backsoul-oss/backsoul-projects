<template>
  <div class="w-screen flex flex-row justify-center h-screen 2xl:overflow-visible sm:overflow-x-hidden" style="width: revert;">
    <div class="md:w-9/12 sm:w-screen sm:overflow-x-hidden" style="overflow-x: clip;">
      <Header />
    <client-only >
     <Nuxt class="mt-6"/>
    </client-only>
    </div>
  </div>
</template>

<script>
import '~/assets/icons'

export default {
  layout: 'default',
}
</script>

<style>
html{
    overflow-x: hidden;
}
</style>
