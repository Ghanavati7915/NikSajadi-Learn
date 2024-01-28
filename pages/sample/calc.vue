
<script setup lang="ts">
definePageMeta({
  layout: 'guest'
})
// let counter = ref(5)
// setTimeout(()=>{
//   counter.value = counter.value + 1;
// },5000)

// let count = ref(0);
// const counter = () => {

//   count.value = count.value + 1;

// }
// const names = ref( ["Aria","Babak", "Araz"]) ;
// const family = ref("karimi");

const numA = ref(0);
const numB = ref(0);
const result = ref(); 

const sumNum = ()=>{
  result.value = +numA.value + +numB.value;
}
const subNum = ()=>{
 result.value =  +numA.value - +numB.value;
}
</script>

<template>
<div>
  <!-- <p @click="counter= 0"> Hello {{ counter }}</p> -->
<!-- <p> {{ count }} </p>
<button type="button" @click= "counter"> click </button>  -->

<!-- <p> salam, {{ names [1] }}</p>
<p> salam, {{ names [2] }}</p> -->

<!-- <p v-for="name in names"> salam, {{ name }}</p> -->
<!-- <p v-for="(name,u) in names" :key="u" :name="u"> salam, {{u+1}} - {{ name }}</p> -->

<!-- <input type="text" v-model="family"> -->
<!-- <p>{{ family }}</p> -->


<p>A : <input type="text" v-model="numA"></p>
<p>B : <input type="text" v-model="numB"></p>
<button type="button" @click= "sumNum">+</button>

<button type=" button" @click="subNum">-</button>
<p>A : {{ numA}}</p>
<p>B : {{ numB}}</p>
<!-- <p>Sum : {{+numA + +numB}}</p> -->
<!-- <p>Sum : {{sumNum()}}</p> -->
<p v-if="result"> result = {{ result }}</p>

<nuxt-link to="/"> back</nuxt-link>
</div>


</template>
