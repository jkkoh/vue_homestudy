<template>
  <div class="home">
    <p>welcome to home</p>
    <p>{{homeValue}}</p>
    <CountComponent v-on:countEvent="updateHomeValue" />
  </div>
</template>

<script>
import CountComponent from "@/components/bClick.vue";



export default {
  name: "HomeComponent",
  components: { CountComponent },
  data: function(){
    return {
      homeValue: 20,
    };
  },
  methods: {
    updateHomeValue(){
      this.homeValue++;
      console.log(this.homeValue);
    },
  },
};
</script>
