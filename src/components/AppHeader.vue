<template lang="">
    <header>
        <div class="logo">
            <img src="../assets/img/dc-logo.png">
        </div>
        <nav class="navbar">
            <ul>
                <li v-for="link in listLink">
                    {{link.content}}
                </li>
                          
            </ul>
        </nav>
    </header>
</template>
<script>
export default {
    data() {
        return {
            listLink:[
                {
                    content:"characters",
                    url:"#"
                },
                {
                    content:"comics",
                    url:"#"
                },
                {
                    content:"movie",
                    url:"#"
                },
                {
                    content:"characters",
                    url:"#"
                },
                {
                    content:"tv",
                    url:"#"
                },
                {
                    content:"games",
                    url:"#"
                },
                {
                    content:"collectibles",
                    url:"#"
                },
                {
                    content:"videos",
                    url:"#"
                },
                {
                    content:"fans",
                    url:"#"
                },
                {
                    content:"news",
                    url:"#"
                },
                {
                    content:"shop",
                    url:"#"
                },
            ]
        }
    },
    
}
</script>
<style lang="scss" scoped>
    @use "../style/partials/variables.scss" as*;
    @use "../style/partials/minxins.scss" as*;


    header{
        width:70%;
        margin:0 auto;
        padding:.5rem;

        ul{
            display:flex;
            list-style-type: none;
        }

        li{
            padding:.5rem;
            text-transform: uppercase;
            font-size:.7rem;
        }
    }


</style>