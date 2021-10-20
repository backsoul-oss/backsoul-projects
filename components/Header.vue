<template>
  <div
    class="hidden md:flex justify-between pt-10 px-10 font-semibold text-xl tracking-wide z-20 bg-white pb-8"
    style="position: fixed;    width: inherit;"
  >
    <div class="grid grid-cols-3 gap-5">
      <NuxtLink to="/about" class="hover:text-orange hover:cursor-pointer md:text-xl sm:text-sm">Sobre mi</NuxtLink>
      <a href="https://backsoul-doc.web.app/" class="hover:text-orange
      hover:cursor-pointer md:text-xl sm:text-sm">Documentación</a>
    </div>
    <div>
      <NuxtLink to="/" class="hover:text-orange hover:cursor-pointer md:text-xl sm:text-sm">Inicio</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',

}
</script>
<style>
a.nuxt-link-exact-active  {
  color:orange;
}
</style>
