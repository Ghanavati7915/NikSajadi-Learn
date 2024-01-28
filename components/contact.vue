<script setup>
const props = defineProps({
  avatar: {
    type: String,
    required: true,
  },
  name: {
    type: String,
    required: true,
  },
  mobile: {
    type: Number,
    required: true,
  },
});

</script>

<template>
    
    <div class="bg-cyan-400 my-4" >
        <div class="grid grid-cols-2 gap-2">
        <img :src="props.avatar" alt="avatar" class="avatar"  />
        <div style="margin: 10px;">
            <p>{{ props.mobile }}</p>
            <p>{{ props.name }}</p>
        </div>
       </div>

        
        
    </div>
</template>
<style>
.avatar {
    width: 50px;
    margin: 15px;
    
}

</style>