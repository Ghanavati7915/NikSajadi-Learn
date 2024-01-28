<template>
  <div class="bg-gray-600" style="padding: 10px;">
        <h1>Page C : </h1>
        <div class="grid grid-cols-4 gap-4">
        <Niko v-for="(item,i) in 5" :key="i"/>
    </div>
    </div>


</template>