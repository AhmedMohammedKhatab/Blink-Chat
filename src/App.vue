<template>
  <v-app>
    <sidebar/>
    <v-content>
      <v-row
        no-gutters
      >
        <v-col md="3" class="d-none d-md-flex">
          <conversations/>
        </v-col>
        <v-col md="9" sm="12">
          <chatbox/>
        </v-col>
      </v-row>
    </v-content>
  </v-app>
</template>

<script>
import sidebar from './components/sidebar'
import conversations from './components/conversations'
import chatbox from './components/chatbox'
// import friends from './components/friends'

export default {
  name: 'App',

  components: {
    sidebar,
    conversations,
    chatbox
    // friends
  },

  data: () => ({
    //
  })
}
</script>

<style>
  /* width */
  ::-webkit-scrollbar {
    width: 10px;
  }

  /* Track */
  ::-webkit-scrollbar-track {
    background: #f1f1f1;
  }

  /* Handle */
  ::-webkit-scrollbar-thumb {
    background: #888;
  }

  /* Handle on hover */
  ::-webkit-scrollbar-thumb:hover {
    background: #555;
  }
</style>
