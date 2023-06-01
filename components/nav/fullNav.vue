<template>
  <div>
    <v-navigation-drawer v-model="drawer" temporary>
      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-view-dashboard" v-for="link in links" :key="link" :href="link.url">{{ link.title }}</v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-system-bar window color="black" class="action-bar">
      <v-btn prepend-icon="mdi-phone" variant="text" class="ma-2" href="tel:6019550080">
        Call 601-955-0080
      </v-btn>
    </v-system-bar>
    <v-app-bar density="compact" position-sticky color="blue-accent-4" class="mb-12">
      <v-app-bar-title>
          <v-img class="ml-n4 ml-md-n12" height="30px" src="/logo.png"></v-img>
      </v-app-bar-title>
      <v-spacer></v-spacer>

      <v-btn @click="toggleTheme" icon="mdi-theme-light-dark" class="mr-3"></v-btn>
      <v-tabs right >
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