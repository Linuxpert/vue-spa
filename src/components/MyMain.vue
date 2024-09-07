<template>
  <div class="containerMain">
    <div class="music">

      <hr class="redBar">

      <h2>
        Music Is Life
      </h2>

      <hr class="bar">

      <p class="descBar">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto tempore dolores fugit maxime! Fuga, eligendi provident culpa ad, iste sint magni quam molestiae officiis error eos molestias, quisquam ipsum fugiat.
      </p>

    </div>

    <div class="bandNews">
      <h2>
        Latest Band News
      </h2>

      <hr class="bar">

      <p class="descBar">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto tempore dolores fugit maxime! Fuga, eligendi provident culpa ad, iste sint magni quam molestiae officiis error eos molestias, quisquam ipsum fugiat.
      </p>

      <div class="containerNews">
        <div class="boxLeft">
          
            
            <div class="techCard">
              <div class="boxHoverLeftHori">
                <h3 class="info">
                  Tecnology and music
                </h3>
              </div>
              <img src="../../src/assets/blog_music_techo.jpg" alt="">
              <h3 class="boxTitle">Tecnology and music</h3> 
              <p class="description">Sed sit amet sem turpis. CUrabitur cursor lacinia est at interdum risus id condimentum.</p>
            </div>
          
          

          <div class="boxMiddle">
            <div class="middleCard">
              <div class="boxHoverLeftVert">
                <h3 class="info">
                  While my guitar gently weeps
                </h3>
              </div>
              <img src="../../src/assets/blog-post3.jpg" alt="">
              <h3 class="boxTitle">While my guitar gently weeps</h3> 
              <p class="description">Sed sit amet sem turpis. CUrabitur cursor lacinia est at interdum risus id condimentum.</p>
            </div>

            <div class="middleCard">
              <div class="boxHoverLeftVert">
                <h3 class="info">
                  It just sounds better
                </h3>
              </div>
              <img src="../../src/assets/blog-post4.jpg" alt="">
              <h3 class="boxTitle">It just sounds better</h3> 
              <p class="description">Sed sit amet sem turpis. CUrabitur cursor lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>

          <div class="rockCard">
            <div class="boxHoverLeftHori">
                <h3 class="info">
                  The flavor of rock
                </h3>
              </div>
            <img src="../../src/assets/blog_flavor_rock-1200x600.jpg" alt="">
            <h3 class="boxTitle">The flavor of rock</h3> 
            <p class="description">Sed sit amet sem turpis. CUrabitur cursor lacinia est at interdum risus id condimentum.</p>
          </div>

        </div>

        <div class="boxRight">
          <div class="oldschoolCard">
            <div class="boxHoverRightVert1">
                <h3 class="info">
                  Taking it back to the old school
                </h3>
              </div>
            <img src="../../src/assets/blog-post1-400x600.jpg" alt="">
            <h3 class="boxTitle">Taking it back to the old school</h3> 
            <p class="description">Sed sit amet sem turpis. CUrabitur cursor lacinia est at interdum risus id condimentum.</p>
          </div>

          <div class="legendCard">
            <div class="boxHoverRightVert2">
                <h3 class="info">
                  Sharing the stage with a legend
                </h3>
              </div>
            <img src="../../src/assets/blog-post2-400x600.jpg" alt="">
            <h3 class="boxTitle">Sharing the stage with a legend</h3> 
            <p class="description">Sed sit amet sem turpis. CUrabitur cursor lacinia est at interdum risus id condimentum.</p>
          </div>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'MyMain',
  components: {
    
  }
}
</script>

<style lang="scss">
// barra musica
.music{
  background-color: rgb(50, 56, 68);
  height: 300px;
}
.redBar{
  border: 10px solid #ea4a56;
  width: 30%;
  margin-right: auto;
  margin-left: auto;
}
h2{
    color: #fefefe;
    text-align: center;
    padding: 60px 0 10px 0;
    font-size: 60px;
  }
.bar{
  border: 1px solid rgb(68, 78, 98);
  width: 25%;
  margin-right: auto;
  margin-left: auto;
  margin-top: 10px ;
}
.descBar{
  text-align: center;
  width: 50%;
  margin: 30px auto;
  color: rgb(125, 123, 141);
}

// parte main immagini

.bandNews{
  background-color: rgb(37, 42, 51);
}
.containerNews{
  margin: 30px auto;
  width: 70%;
  display: flex;
  justify-content: center;
}
.boxLeft{
  display: flex;
  flex-direction: column;
  width: 60%;
  
}
// hover img
.boxHoverLeftHori{
  background-color: #ea4a56;  
  position: absolute;
  width: 799px;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  .info{
    color: #fefefe;
  }
}

.boxHoverLeftVert{
  background-color: #ea4a56;  
  position: absolute;
  width: 383px;
  height: 440px;
  display: flex;
  justify-content: center;
  align-items: center;
  .info{
    color: #fefefe;
  }
}

.boxHoverRightVert1{
  background-color: #ea4a56;  
  position: absolute;
  width: 333px;
  height: 510px;
  display: flex;
  justify-content: center;
  align-items: center;
  .info{
    color: #fefefe;
  }
}

.boxHoverRightVert2{
  background-color: #ea4a56;  
  position: absolute;
  width: 333px;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  .info{
    color: #fefefe;
  }
}



.techCard{
  width: 100%;
  background-color: rgb(50, 56, 68);
  img{
    position: relative;
    object-fit: cover;
    width: 100%;
    height: 200px;
    &:hover{
      opacity: .5;
    }
  }
  
}
.boxMiddle{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.middleCard{
  margin-top: 30px;
  width: 48%;
  background-color: rgb(50, 56, 68);
  img{
  position: relative;
  object-fit: cover;
  width: 100%;
  height: 440px;
  &:hover{
      opacity: .5;
    }
  }
}
.rockCard{
    margin-top: 30px;
    background-color: rgb(50, 56, 68);
    width: 100%;
    img{
      position: relative;
      object-fit: cover;
      width: 100%;
      height: 200px;
    &:hover{
      opacity: .5;
      }
    }
}
.boxRight{
  display: flex;
  flex-direction: column;
  width: 25%;
  justify-content: space-between;
  margin-left: 30px ;
}
.oldschoolCard{
  background-color: rgb(50, 56, 68);
  width: 100%;
  img{
      position: relative;
      object-fit: cover;
      width: 100%;
      height: 510px;
      &:hover{
      opacity: .5;
      }
    }
}
.legendCard{
  background-color: rgb(50, 56, 68);
  width: 100%;
  img{
      position: relative;
      object-fit: cover;
      width: 100%;
      height: 400px;
      &:hover{
      opacity: .5;
      }
    }
}
.boxTitle{
  color: #ea4a56;
  margin: 15px 0 5px 10px;
}
.description{
  color: #7d7b8d;
  margin: 0 0 10px 10px;
}

</style>
