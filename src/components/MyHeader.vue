<template>
  <div id="containerHeader">
    <div class="logoMenu">
        <img src="../../src/assets/avada-music-logo.png" alt="">

        <Slide right width="1918">
            <MenuSett v-for="link, i in links" :key="i" :details="link"/>
        </Slide>
        
    </div>

    <div class="center">
        <h1>
            <strong>
                Untold Stories
            </strong>
        </h1>

        <span class="subtitle">
            There is an untold story behind every favorite song.
        </span>

        <div class="headerBtn">
            <div class="album">
                <span>
                    LATEST ALBUM
                </span>
            </div>

            <div class="dates">
                <span>
                    LIVE DATES
                </span>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import { Slide } from 'vue-burger-menu'
import MenuSett from '@/components/MenuSett.vue'

export default {
  name: 'MyHeader',
  components: {
    Slide,
    MenuSett
  },
  data(){
      return {
             links: [
                {
                    text: "Home",
                    urls:"#"
                },
                {
                    text: "Meet The Band",
                    urls:"#"
                },
                {
                    text: "Live Dates",
                    urls:"#"
                },
                {
                    text: "Latest News",
                    urls:"#"
                },
                {
                    text: "Albums",
                    urls:"#"
                },
                {
                    text: "Fans",
                    urls:"#"
                },
             ]
      }
  }
}
</script>

<style  lang="scss">

#containerHeader {
  background-image: url(../../src/assets/home_slider.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  height: 100vh;

  .logoMenu{
      display: flex;
      justify-content: space-between;
      align-items: center;
      img {
          margin: 20px;
          z-index: 1001;
      }
    
  }
    .center{
      text-align: center;
      margin-top: 10%;
      h1{
          font-size: 160px;
          color: #fefefe;
          font-family: 'Roboto', sans-serif;
      }
      .subtitle{
          font-size: 20px;
          color: #fefefe;
      }
  }
  

  .headerBtn{
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 30px;
      .album{
          margin-right: 20px;
          padding: 10px 30px;
          background-color: #ea4a56;
          color: #fefefe;
          &:hover{
              background-color: #fefefe;
              color: #272b34;
              cursor: pointer;
          }
      }
      .dates{
          margin-right: 20px;
          padding: 10px 30px;
          border: 1px solid #fefe;
          color: #fefe;
          &:hover{
              background-color: #fefefe;
              color: #272b34;
              cursor: pointer;
          }
      }
  }
    
}

</style>
