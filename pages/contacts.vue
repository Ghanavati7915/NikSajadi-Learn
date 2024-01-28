<script setup>

const contactsList = ref([
{name:"Ali",mobile:"091747875555",avatar:"https://avatar.iran.liara.run/public/boy"},
{name:"Nazanin",mobile:"09185555555",avatar:"https://avatar.iran.liara.run/public/girl"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
{name:"Majid",mobile:"09125556565",avatar:"https://avatar.iran.liara.run/public"},
])

</script>

<template>
    <div class = "bg-cyan-200 p-5">
        <!-- <contact v-for="(item,i) in 4 " :key="i" /> -->

        <contact v-for="(contact,i) in contactsList" 
        :key="`contact_${i}`" 
        :avatar="contact.avatar" 
        :name="contact.name" 
        :mobile="contact.mobile" />

        <nuxt-link to="/">Number </nuxt-link>
        
    </div>
</template>
<style></style>