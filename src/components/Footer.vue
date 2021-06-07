<template>
    <section> 
        <div class="section-links">
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
        <div class="section-sign"></div>

    </section> 
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>
    section {

        background-image: url('../assets/images/footer-bg.jpg')
    }
    .section-links {
        width:70%;
        margin:0 auto;
        display:flex;
        justify-content:space-between;

        .links{
            display:flex;
            justify-content: space-between;

            .left,
            .middle,
            .right {
                margin-right: 20px;
                
                h3 {
                    padding-top: 20px;
                    color:white;
                    text-transform:uppercase;
                }
            }
        }
    }
  

    ul{
        list-style: none;

        li{
            padding-top: 2px;

           a{
            color:rgb(175, 175, 175);
            text-decoration:none;
            font-size: 12px;
           } 
        }
    }

</style>