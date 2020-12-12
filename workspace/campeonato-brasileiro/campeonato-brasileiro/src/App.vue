<template>
  <v-app>
    <AppTopBar/>
    
    <v-main>
       <PaginaPrincipal/>
    </v-main>
  </v-app>
</template>

<script>

import PaginaPrincipal from './components/PaginaPrincipal'
import AppTopBar from './components/shared/AppTopBar'

export default {
  name: 'App',
  components: {
    PaginaPrincipal,
    AppTopBar,
  }
};
</script>

