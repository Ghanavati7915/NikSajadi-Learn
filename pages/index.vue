<script setup>
const colorMode = useColorMode()

const isDark = computed({
  get () {
    return colorMode.value === 'dark'
  },
  set () {
    colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark'
  }
})
</script>


<template>
    <div style="background-color: white;padding: 10px;">
        <h1>Hello 1 </h1>

        <ClientOnly>
    <UButton
      :icon="isDark ? 'i-heroicons-moon-20-solid' : 'i-heroicons-sun-20-solid'"
      color="gray"
      variant="ghost"
      aria-label="Theme"
      @click="isDark = !isDark"
    />

    <template #fallback>
      <div class="w-8 h-8" />
    </template>
  </ClientOnly>


        <nuxt-link to="A"> Page A</nuxt-link>
        <span> | </span>
        <nuxt-link to="B"> Page B</nuxt-link>
        <span> | </span>
        <nuxt-link to="C"> Page C</nuxt-link>
        <span> | </span>
        <nuxt-link to="sample/calc"> Page Calc</nuxt-link>
        <span> | </span>
        <NuxtLink to="contacts"> Contacts </Nuxtlink>

    </div>
    
</template>