<template>
  <v-app>
    <v-toolbar>
      <v-toolbar-side-icon @click.native.stop="sideNav = !sideNav" class="hidden-sm-and-up"></v-toolbar-side-icon>
      <v-toolbar-title>DevMeetup</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn flat><v-icon left >supervisor_account</v-icon>Meetups</v-btn>
        <v-btn flat><v-icon left>create</v-icon>New</v-btn>
        <v-btn flat><v-icon left>face</v-icon>Profiles</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <!-- <v-content> -->
      <v-container grid-list-md text-xs-center>
        <v-layout row wrap>
          <v-flex xs12>
            <v-card dark>
              <v-card-text class="px-0">12</v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    <!-- </v-content> -->
    <v-navigation-drawer v-model="sideNav">
      <v-list>
        <v-list-tile>
          <v-list-tile-action>
            <v-icon>supervisor_account</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>Meetups</v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <main>

    </main>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      sideNav: false
    }
  },
  name: 'App'
}
</script>
