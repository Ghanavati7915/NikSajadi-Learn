<script setup>
</script>

<template>
<div  style="background-color: green;padding: 10px;">
    <h1>  A Page </h1>
    <comup v-for="(item,i) in 3" :key="i"/>
     <nuxt-link to ="/">back</nuxt-link>
    
</div>
</template>

<style>

</style>