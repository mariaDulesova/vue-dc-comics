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
*{
  margin:0;
  padding:0;
  box-sizing: border-box;
}

</style>
