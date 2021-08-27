<template>
  <form @submit.prevent="onSubmit">
  <p class="container">
    <label class="label" form="first_name">First Name:</label>
    <input class="inputfield" id="first_name" v-model="first_name">
  </p>
  <p class="container">
    <label class="label" form="last_name">Last Name:</label>
    <input class="inputfield" id="last_name" v-model="last_name">
  </p>
  <p class="container">
    <label class="label" form="group">Age:</label>
    <select class="inputfield" id="group" v-model="age">
    <option  v-for="age of validAges" :key="age">{{age}}</option>
    </select>
  </p>
  <p class="container">
  <input id="submit-button" class="button" type="submit" value="Submit">
  </p>
 </form>
  </template>


  <script>
  export default {
    name: 'RegistrationForm',
    data() {
      return {
        first_name: '',
        last_name: '',
        age: undefined,
        validAges: [17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,34,35]
      }
    },
    methods: {
      onSubmit() {
         alert(`${this.last_name} ` + `${this.first_name} is ` + `${this.age}`); 
      },
    }
  }

  </script>

<style>
.container {
   text-align: left;
}
.label {
    padding: 5px;
    text-align: left;
    width: 80%;
    margin: 5px;
    font-family: sans-serif Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    font-size: 40px;
}
.inputfield {
    padding: 5px;
    background: rgb(205, 221, 236);
    font-family: sans-serif Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    font-size: 40px;
}
.button {
    padding: 10px;
    background: turquoise;
    font-size: 40px;

}

</style>
