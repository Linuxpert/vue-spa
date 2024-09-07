<template>
  <div>
    <a class="burger" :href="details.urls">
    <span class="menu">{{details.text}}</span>
    </a>
  </div>
</template>

<script>


export default {
  name: 'MenuSett',
  props:{
      details:Object
  },
  components: {
    
  },
  
}
</script>

<style  lang="scss">
    .bm-menu{
        background-color: #ea4a56;
    }
    .burger{
        justify-content: center;
        align-items: center;
        margin-top: 20px;
        text-decoration: none;
    }
    .menu{
        font-size: 40px;
        // color: #fefefe;
        color: rgb(248, 149, 158);
        &:hover{
           color: #fefefe; 
        }
    }
    .bm-item-list{
        margin: 10% 0 0 0;
    }
    .bm-cross-button{
        right: 36px !important;
        top: 36px;
    }
    .bm-cross{
        width: 2px !important;
        height: 35px !important;
    }
    .bm-burger-bars{
        background-color: #fefefe;
    }
    .bm-item-list>*{
        justify-content: center;
        align-items: center;
    }
</style>
