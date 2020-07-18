<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
     <div>
  <VueToggles
  @click="value = !value"
  :value="value"
  height="30"
  width="90"
  checkedText="On"
  uncheckedText="Off"
  checkedBg="#b4d455"
  uncheckedBg="lightgrey"
       />
  </div>

   
  <VueToggles
  @click="value = !value"
  :value="value"
  height="30"
  width="90"
  checkedText="On"
  uncheckedText="Off"
  checkedBg="#b4d455"
  uncheckedBg="lightgrey"
       />

       <anchored-heading :level="1">Hello this is my world!</anchored-heading>
  
  </div>

 

  
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

import VueToggles from 'vue-toggles';

import AnchorHeader from "@/components/MyCustomComponent"

export default {
  name: "Home",
  components: {
    HelloWorld,
    VueToggles,
    "anchored-heading": AnchorHeader

  }
};
</script>
