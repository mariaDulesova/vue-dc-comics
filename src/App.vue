<template>
  <div id="app">
    
    <!-- Header -->
    <Header/>
    <!-- /Header -->

    <!-- Main -->
    <main>
      <Content/>

    </main>
    <!-- /Main -->

    <!-- Footer -->
    <Footer/>
    <!-- /Footer -->

  </div>
</template>

<script>
import Header from './components/Header';
import Content from './components/Content';
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Footer
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@300;400;500;600;700&family=Oswald:wght@300;400;500;600;700&display=swap');

*{
  margin:0;
  padding:0;
  box-sizing: border-box;
}

html {
  font-size: 15px;
}

body {
  font-family: 'Oswald', sans-serif;
}

</style>
