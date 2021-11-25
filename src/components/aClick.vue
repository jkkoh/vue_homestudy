<template>
    <div>
        <p>welcome to bClick.vue</p>
        <p>{{this.clickValue}} : 상위 about.vue 에서 받아온 값</p>
    </div>
</template>
<script>
export default {
    name: "ClickComponent",
    props: ["clickValue"],
};
</script>