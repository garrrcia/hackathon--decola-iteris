<template>
  <div class="app-top-bar">
    <v-app-bar app color="teal accent-4">
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-toolbar-title> Campeonato Brasileiro ⚽ </v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list nav dense>
        <v-list-item-group v-model="group" active-class="deep-teal--text text--accent-4">
         
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-whistle</v-icon>
            </v-list-item-icon>
            <v-list-item-title>
                Página principal
            </v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-soccer</v-icon>
            </v-list-item-icon>
            <v-list-item-title>
                Classificação
            </v-list-item-title>
          </v-list-item>

        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: 'AppTopBar',

  data() {
    return {
        drawer: false,
        group: null,
    }
  }
};
</script>
