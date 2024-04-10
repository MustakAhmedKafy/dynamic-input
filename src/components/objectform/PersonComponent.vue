<script setup>
const props = defineProps(["person"]);
</script>
<template>
  <div>
    <label for="">Name</label> <br />
    <input type="text" v-model="person.name" /> <br />
    <br />

    <label for="">Email</label> <br />
    <input type="text" v-model="person.email" /> <br />
  </div>
</template>
