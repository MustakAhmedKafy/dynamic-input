<script setup>
import PersonComponent from "../objectform/PersonComponent.vue";
import { reactive } from "vue";

const person = reactive({
  name: "Ahmed Mustak",
  email: "mustak@gmail.com",
});
</script>
<template>
  <div>
    <p>{{ person.name }}</p>
    <p>{{ person.email }}</p>
    <PersonComponent :person="person" />
  </div>
</template>
