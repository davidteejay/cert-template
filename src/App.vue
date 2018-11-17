<template>
  <v-app>
    <Loader :active="loading"/>
    <!-- <div class="cert-cover">
      <Cert1/>
    </div>  
    <div class="cert-cover">
      <Cert2/>
    </div> 
    <div class="cert-cover">
      <Cert3/>
    </div>     -->
    <Error/>
  </v-app>
</template>

<script>
import Cert1 from './components/Cert1'
import Cert2 from './components/Cert2'
import Cert3 from './components/Cert3'
import Loader from './components/Loader'
import Error from './components/Error'

export default {
  name: 'App',
  components: {
    Cert1,
    Cert2,
    Cert3,
    Loader,
    Error
  },
  data () {
    return {
      loading: false
    }
  }
}
</script>

<style lang="css">
@import './assets/css/style.css';
</style>

