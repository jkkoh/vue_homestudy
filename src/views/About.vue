<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p>하위 컴포넌트로 데이터 값을 보내줍니다</p>
    <ClickComponent v-bind:clickValue="aboutValue"/>
  </div>
</template>

<script>
import ClickComponent from "@/components/aClick.vue";
export default {
  name: "AboutComponent",
  components: { ClickComponent },
  data (){
    return{
      aboutValue : 10,
    };
  },
}
</script>
