<template>
  <div >
        <keep-alive>
              <component :is="conteudo" />
        </keep-alive>
  </div>
</template>

<script>

import About from '../views/About.vue'
import Home from '../views/Home.vue'
import Projects from '../views/Projects.vue'
export default {
      name: 'Conteudo',
      props:{
              conteudo:{
                type:String,
                required: true
            }
      },
      components:{
              About,
              Home,
              Projects
      },

}
</script>

<style scoped>


</style>