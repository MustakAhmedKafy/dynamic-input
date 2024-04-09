<script setup>
import TextArea from "./TextArea.vue";
import { ref } from "vue";
const name = ref("Mustak Ahmed");
const email = ref("ahmedmustak99@gmail.com");
</script>
<template>
  <div>
    <h5>Original Name: {{ name }}</h5>
    <h5>Original Email: {{ email }}</h5>
    <br />

    <h6>Two way binding</h6>
    <input type="text" v-model="name" /> <br />
    <br />
    <TextArea label="Name" v-model="name" /> <br />
    <TextArea label="Email" v-model="email" />
    <!-- dynamic -->
  </div>
</template>
