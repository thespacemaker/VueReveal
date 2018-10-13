<template>
  <v-app>
    <v-navigation-drawer
      persistent
      :mini-variant="miniVariant"
      :clipped="clipped"
      v-model="drawer"
      enable-resize-watcher
      fixed
      app
    >
      <v-list>
        <v-list-tile
          value="true"
          v-for="(item, i) in items"
          :key="i"
          v-bind:to="item.to"
        >
          <v-list-tile-action>
            <v-icon v-html="item.icon"></v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar
      app
      :clipped-left="clipped"
    >
      <v-toolbar-side-icon outline color="primary" @click.stop="drawer = !drawer"></v-toolbar-side-icon>
      <v-toolbar-title>Adnan's Slides</v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <v-content>
      <router-view/>
    </v-content>
    <v-footer style="background-color:#351652" id="shadow" fixed>
        <v-layout row wrap align-center>
          <v-flex xs12>
            <div class="white--text ml-3 text-xs-center">
              Made with
              <v-icon color="white">fas fa-heart</v-icon>
              by <a class="white--text" href="theadnan.tech" target="_blank">    TheSpaceMaker</a>
            </div>
          </v-flex>
        </v-layout>
      </v-footer>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        {
          icon: 'fas fa-laptop',
          title: 'Slides',
          to: '/'
        },
        {
          icon: 'fas fa-user-astronaut',
          title: 'About Me',
          to: '/about'
        },
        {
          icon: 'fas fa-phone',
          title: 'Contact',
          to: '/Contact'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
