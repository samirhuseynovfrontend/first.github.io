<template>
  <v-app>
    <navbar></navbar>
    <router-view/>
  </v-app>
</template>
<script>

import Navbar from '@/components/Navbar'
import Home from './views/Home'
import Gallery from './views/Gallery'
import About from './views/About'

export default {
  components:{
    Navbar,Home,Gallery,About
  }

}
</script>
<style lang="stylus">

</style>
