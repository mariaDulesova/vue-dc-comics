<template>
    <nav>
        <img src="@/assets/images/dc-logo.png" alt="Logo">
        <ul>
            <li v-for = '(link,index) in links' :key='index'>
                <a :href='link.url' :class='{active: link.current}'> {{ link.text }} </a>
            </li>
        </ul>

    </nav>
</template>

<script>
export default {
    name: 'Header',
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
            ]
        }
    }
}
</script>

<style scoped lang="scss">
nav {
    width:70%;
    margin:0 auto;
    padding: 15px 0;
    display:flex;
    justify-content: space-between;
    align-items: center;
    
}
ul {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    list-style: none;

    li{
        a{
            text-decoration: none;
            text-transform: uppercase;
            padding: 10px;
            color: black; 
        }
        .active{
            color: #0E7CEC;
            border-bottom: 3px solid #0E7CEC;
            
        }
    }
}


</style>