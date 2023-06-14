<template>
  <div>
    <v-navigation-drawer v-model="drawer" temporary>
      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-view-dashboard" v-for="link in links" :key="link" :href="link.url">{{ link.title }}</v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar flat scroll-behavior="hide" color="black" class="mb-0 pb-0 text-right">
      <v-spacer></v-spacer>
      <v-btn right prepend-icon="mdi-phone" variant="text" class="pa-2" href="tel:4065774131">
        Call Wes at 406-577-4131
      </v-btn>
    </v-app-bar>
    <v-app-bar density="compact" position-sticky color="blue-accent-4" class="mb-12">
      <v-app-bar-title>
          <v-img class="ml-n4 ml-md-n12" height="30px" src="/logo.png"></v-img>
      </v-app-bar-title>
      <v-spacer></v-spacer>

      <v-btn @click="toggleTheme" icon="mdi-theme-light-dark" class="mr-3"></v-btn>
      <v-tabs right class="d-none d-md-flex">
        <v-tab class="pb-n15" color="white" v-for="link in links" :key="link" :to="link.url"> {{ link.title }} </v-tab>
      </v-tabs>

      <v-app-bar-nav-icon class="d-lg-none" variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>
  </div>
</template>

<style lang="scss">
.action-bar {
  height: 50px;
}
</style>

<script>
import { useTheme } from 'vuetify'

export default {
  setup() {
    const theme = useTheme()

    return {
      theme,
      toggleTheme: () => theme.global.name.value = theme.global.current.value.dark ? 'light' : 'dark'
    }
  },
  data: () => ({
    drawer: null,
    links: [
      {
        title: "Home",
        url: "/",
        icon: "mdi-home"
      },
      {
        title: "Services",
        url: "services",
        icon: "mdi-home"
      },
      {
        title: "About",
        url: "about"
      },
      {
        title: "Contact",
        url: "contact"
      }
    ]
  })
}
</script>