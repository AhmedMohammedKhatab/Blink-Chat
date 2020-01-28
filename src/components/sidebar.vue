<template>
  <v-navigation-drawer
    color="#48B0B8"
    mini-variant
    v-model="side"
    app
    permanent
    touchless
    dark
  >
    <v-list
      dense
      nav
      class="py-0"
    >
      <v-list-item class="px-0">
        <v-list-item-avatar>
          <img src="https://i.pinimg.com/originals/60/d4/d3/60d4d31e4f2b18abaee11da6281ff6ea.png">
        </v-list-item-avatar>
      </v-list-item>

      <v-list-item
        v-for="item in items"
        :key="item.icon"
        link
      >
        <v-icon>{{ item.icon }}</v-icon>
      </v-list-item>
    </v-list>
    <template v-slot:append>
    <div class="pa-2">
      <v-btn icon>
        <v-icon>mdi-logout</v-icon>
      </v-btn>
    </div>
    </template>
  </v-navigation-drawer>
</template>

<script>
export default {
  data () {
    return {
      side: true,
      items: [
        { icon: 'mdi-forum-outline' },
        { icon: 'mdi-account-outline' },
        { icon: 'mdi-settings-outline' }
      ]
    }
  }
}
</script>
