<script setup>
import PersonComponent from "../objectform/PersonComponent.vue";
import TextArea from "../TextArea.vue";
import { reactive } from "vue";

const person = reactive({
  name: "Ahmed Mustak",
  email: "mustak@gmail.com",
});
</script>
<template>
  <div>
    <p>Name: {{ person.name }}</p>
    <p>Email: {{ person.email }}</p>
   
      <label for="">Your name</label> <br>
      <input type="text" v-model="person.name">

   <br> <br>
    <PersonComponent :person="person" />

    <!-- more dynamic -->

    <h2>more dynamic</h2>
    <br />

    <TextArea label="name" v-model="person.name" />
    <TextArea label="email" v-model="person.email" />
  </div>
</template>
