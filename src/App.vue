<template>
  <div id="app">
    <MyHeader/>

    <MyMain/>

    <MyFooter/>


  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@1,300;1,400&family=Roboto:wght@900&family=Ubuntu:wght@300;500&display=swap');
</style>
