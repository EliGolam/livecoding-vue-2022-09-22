<template>
<div class="background">

</div>
</template>

<script>
export default {
    name: "ContentComponent",
}
</script>

<style lang="scss" scoped>
$clr: greenyellow;

@mixin baseShape {
    margin: 0 auto;
    padding: 20px;
    width: 100%;
    aspect-ratio: 16 / 9;
    object-fit: cover;
}



.background {
    @include baseShape();
    background-image: url("../assets/logo.png");
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center;
    background-color: $clr;
}
</style>