<template>
    <div>
        <p>------------------------</p>
        <p>welcome to bClick.vue</p>
        <button @click = "updateHomeValue">클릭시 값이 증가합니다</button>
    </div>
</template>
<script>
export default {
    name: "CountComponent",
    methods: {
        updateHomeValue(){
            this.$emit("countEvent");
        },
    },
}
</script>