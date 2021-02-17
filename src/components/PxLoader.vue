<template>
    <div class="loader -mt-16 flex items-center justify-center">
        <pulse-loader :color="'#d4d4d4'" :size="40"></pulse-loader>
    </div>
</template>

<script>
export default {
    name: "PxLoader"
}
</script>

<style scoped>
.loader {
    width: 100%;
    height: 100vh;
    position: absolute;
    z-index: 100;
    background-color: white;
}
</style>