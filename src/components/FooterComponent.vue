<template>
<footer>

</footer>
</template>

<script>
export default {
    name: "FooterComponent",
}
</script>

<style lang="scss" scoped>
$clr: cyan;

@mixin baseShape {
    margin: 0 auto;
    padding: 20px;
    width: 100%;
    aspect-ratio: 16 / 9;
    object-fit: cover;
}

footer {
    @include baseShape();
    background-color: $clr;
    margin-top: 2rem;
}
</style>