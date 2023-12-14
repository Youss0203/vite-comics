<template lang="">
    
    <article class="content-here">
        <div class="main-content">
        <i class="fa-solid fa-arrow-right"></i>
        <h1>Content goes here</h1>
        <i class="fa-solid fa-arrow-left"></i>
        </div>
    </article>


</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
@use "../style/partials/variables.scss" as*;
@use "../style/partials/minxins.scss" as*;


article.content-here {
    height: 130px;
    background-color: black;
    color: white;

    div.main-content{
        width:70%;
        margin:0 auto;
    
        h1{
            padding: 0 .4rem;
        }
    }
}

</style>