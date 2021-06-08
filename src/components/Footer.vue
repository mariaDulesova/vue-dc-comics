<template>
    <section> 
        <div class="section-services">
            <Bonus/>
        </div>
        <div class="section-links wrap">
            <div class= "links">
                <div class="left">
                    <h3>DC Comics</h3>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>

                </div>
                <div class="middle">
                    <h3>DC</h3>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops </a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="right">
                    <h3>Sites</h3>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
            <img src="../assets/images/dc-logo-bg.png" alt="">
        
        </div>
        <div class="section-sign">
            <div class="bottom-links wrap">
                <div class="button">
                    <a href="#">Sign-Up Now!</a>
                </div>
                <div class="socials">
                    <h3>Follow Us</h3>
                    <img src="../assets/images/footer-facebook.png" alt="Facebook">
                    <img src="../assets/images/footer-twitter.png" alt="Twitter">
                    <img src="../assets/images/footer-youtube.png" alt="Youtube">
                    <img src="../assets/images/footer-pinterest.png" alt="Pinterest">
                    <img src="../assets/images/footer-periscope.png" alt="Periscope">
                </div>
            </div>
        </div>

    </section> 
</template>

<script>
import Bonus from "./Bonus"
export default {
    name: "Footer",
    components: {
        Bonus
    }
}
</script>

<style lang="scss" scoped>

    @import "../style/variables.scss";
    @import "../style/mixins.scss";

    section {
        position:relative;
        background-image: url("../assets/images/footer-bg.jpg");

        .wrap {
          @include wrap;
        }

         .section-links { 
            @include flex-align-center;
            justify-content:space-between;

            .links {
                display:flex;
                justify-content: space-between;
                .left,
                .middle,
                .right {
                    margin-right: 20px;

                    h3 {
                        color:$primary-white;
                        text-transform:uppercase;
                    }

                    ul {
                        list-style: none;
                        padding-bottom: 20px;

                        li {
                            a {
                                color:rgb(175, 175, 175);
                                text-decoration:none;
                                font-size: 0.8rem;
                            } 
                        }
                    }
                }
            }

            img {
                width: 500px;
            }
        }
        
        .section-sign {
            position:absolute;
            left:0;
            bottom:0;
            width: 100%;
            background-color: $primary-dark-gray;
            padding: 15px 0;

            .bottom-links{
                @include flex-align-center;
                justify-content: space-between;

                .button {
                
                    a {
                        padding: 10px;
                        border: 2px solid $primary-blue;
                        color: $primary-white;
                        text-decoration:none;
                        text-transform: uppercase;
                    }
                }

                .socials{
                    @include flex-align-center;
                
                    img,h3{
                        padding: 10px;
                    }

                    h3 {
                        text-transform: uppercase;
                        color: $primary-blue;
                    }

                }
            }
        }

        .section-services {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            background-color: $primary-blue;


        }
    }

</style>