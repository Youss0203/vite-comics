<template lang="">
    <section class="hero"></section>
    <section class="social"></section>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    @use "../style/partials/variables.scss" as*;
    @use "../style/partials/minxins.scss" as*;

    section.hero{
        height:471px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: 100%;
        background-repeat: no-repeat;
    }

    section.social{
        height:119px;
        background-color: #303030;
    }
</style>