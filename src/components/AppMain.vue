<template lang="">

    <div >
        <img class="jumbo" src="../assets/img/jumbotron.jpg" alt="">
    </div>
    <div class="container">
        <div class=" w-70">
            <button class="current">CURRENT SERIES</button>
        </div>
        <div class="w-70">
            <article v-for="list in comicList" :imageSrc="list.thumb" :title="list.series">
            <img :src="list.thumb" alt="">
            <p>{{list.series}}</p>
        </article>
        </div>
        <div class="btn">
        <button>LOAD MORE</button>
        </div>
    </div>

</template>
<script>
export default {
    
    data() {
        return {
            comicList: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@use "../style/partials/variables.scss" as*;
@use "../style/partials/minxins.scss" as*;


article{
    width: calc((100% / 6) - .5rem);
    align-items: stretch;
    margin-bottom:1rem;
    margin-right:.25rem;
    margin-left: .25rem;

    div.main-content {
        width: 70%;
        margin: 0 auto;

        h1 {
            padding: 0 .4rem;
        }
    }

}

.jumbo {
    height: 300px;
    object-fit: cover;
    object-position: top;
    width: 100%;
    display: block;
}

div.container{
    background-color: black;
    position:relative;

    .w-70{
        width: 70%;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        padding:1rem;
    }
}
p{
    color:white;
    text-align:center;
    text-transform: uppercase;
    font-size:.7rem;
}
img{width: 100%;
height: 200px;}

button{
    padding:.5rem 2rem;
    background-color: #027FF0;
    border:none;
    color:white;
    margin-bottom:2rem;
}

.btn{
    display: flex;
    justify-content: center;
    align-items: center;
    

}
.current{
    position: absolute;
    top: -15px;
}
</style>