<template>
    <nav>
        <div class="wrap">
            <img src="@/assets/images/dc-logo.png" alt="Logo">
            <ul>
                <li v-for = '(link,index) in links' :key='index'>
                    <a 
                    :href='link.url' 
                    :class='(activeIndex==index) ? "active" : ""'
                    @click = 'getActiveLink(index)'> {{ link.text }} </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name: "Header",
    data:function() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#characters',
                    current:false
                },
                {
                    text: 'Comics',
                    url: '#comics',
                    current:true
                },
                {
                    text: 'Movies',
                    url: '#movies',
                    current:false
                },
                {
                    text: 'TV',
                    url: '#tv',
                    current:false
                },
                {
                    text: 'Games',
                    url: '#games',
                    current:false
                },
                {
                    text: 'Collectibles',
                    url: '#collectibles',
                    current:false
                },
                {
                    text: 'Videos',
                    url: '#videos',
                    current:false
                },
                {
                    text: 'Fans',
                    url: '#fans',
                    current:false
                },
                {
                    text: 'News',
                    url: '#news',
                    current:false
                },
                {
                    text: 'Shop',
                    url: '#shop',
                    current:false
                }
            ],

            activeIndex: 0,
        }
    },
    methods: {
        getActiveLink: function(i) {
            return this.activeIndex = i;
            
        }
    }
}
</script>

<style scoped lang="scss">

    @import "../style/variables.scss";
    @import "../style/mixins.scss";

    nav {
        padding: 15px 0;
        
        .wrap {
            @include wrap;
            @include flex-align-center;
            justify-content: space-between;
        }
        
    }
    ul {
        @include flex-align-center;
        justify-content: flex-end;
        list-style: none;

        li {
            a {
                text-decoration: none;
                text-transform: uppercase;
                padding: 55px 10px;
                color: $primary-dark-gray; 
        
            }
            .active{
                color: $primary-blue;
                position: relative;

                &::before{
                    content : "";
                    position: absolute;
                    left: 50%;
                    bottom: 0;
                    width: 50%; 
                    border-bottom: 4px solid $primary-blue;
                    transform: translateX(-50%);
                }
            }
        }
    }


</style>