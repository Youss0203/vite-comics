<template lang="">
    <section class="hero">
        <div class="container">
        <div class="navigation">
            

            <nav id="dc-comics">
                <h3>DC COMICS</h3>
                <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Tv</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li class="news">News</li>
                </ul>

                <h3>SHOP</h3>
                <ul>
                    <li>Shop DC</li>
                    <li>Shop DC collectibles</li>
                </ul>
            </nav>
            <nav id="dc">
                <h3>DC</h3>
                <ul>
                    <li>Terms of use</li>
                    <li>Privacy Policy (new)</li>
                    <li>Ad Choises</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscription</li>
                    <li>Talent Workshop</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
            </nav>
            <nav id="sites">
                <h3>SITES</h3>
                <ul>
                    <li>DC</li>
                    <li>Mad Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </nav>

        </div>
        
        <div class="logo">
            <img src="../assets/img/dc-logo-bg.png">
        </div>
    </div>
    </section>
    <section class="social">
        <div class="container">
            <div class="sign">
                <button>SIGN UP NOW!</button>
            </div>

            <div class="socials">
                <p>Follow Us</p>
                <img class="social-logo" src="../assets/img/footer-facebook.png" alt="logo facebook">
                <img class="social-logo" src="../assets/img/footer-twitter.png" alt="logo twitter">
                <img class="social-logo" src="../assets/img/footer-youtube.png" alt="logo youtube">
                <img class="social-logo" src="../assets/img/footer-pinterest.png" alt="logo pinterest">
                <img class="social-logo" src="../assets/img/footer-periscope.png" alt="logo periscope">
            </div>
        </div>
    </section>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
@use "../style/partials/variables.scss" as*;
@use "../style/partials/minxins.scss" as*;

section.hero {
    height: 471px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: 100%;
    background-repeat: no-repeat;
}

section.social {
    padding:2rem;
    background-color: #303030;

}
H3{
    color:white
}
li{
    color:#7C7C7C;
    list-style-type: none;
    font-size:.7rem;
}

#dc-comics,#dc{
    margin-right:1.5rem;
}

.news{
    margin-bottom:.5rem;
}
div.container{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 70%;
  margin: 0 auto;
}
div.sign,.socials{
    display: flex;
    justify-content: center;
    align-items: center;

    button{
    border: #027FF0 2px solid;
    background-color: #303030;
    color:white;
    padding:1rem;
   }
p{
    color:#027FF0;
    text-transform: uppercase;
    margin-right: 1rem;
    font-weight: bold;
}

}
.social-logo{
    margin-right: 1rem;
}
</style>