<script setup>
  import HelloWorld from './components/HelloWorld.vue';
  import CustomInput from './components/CustomInput.vue';
</script>

<template>
  <HelloWorld msg="Vite + Vue" />
  <div class="row">
    <CustomInput 
      text="Name"
      size="col-md-5"
    />
  </div>
</template>
