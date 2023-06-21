<template>
  <v-footer fluid class="ma-0 pa-0 position-sticky">
    <v-row no-gutters align="center" class="px-3 py-5 bg-black w-100 justify-space-between">
      <v-col>
        <p class="skd-logo-font">
          &copy; {{ new Date().getFullYear() }} — McKenzie Law.
        </p>
      </v-col>
      <v-spacer></v-spacer>
      <v-col class="d-flex align-end flex-column">
          <v-chip
            class="ma-2"
            label
            href="mailto:wes@mckenzielawpllc.com">
            <v-icon start icon="mdi-email"></v-icon>
            wes@mckenzielawpllc.com
          </v-chip>
      </v-col>
    </v-row>
  </v-footer>
</template>

<style lang="scss">
.v-footer {
  padding: 0;
}

.skd-logo-font {
  font-family: Play;
}
</style>
