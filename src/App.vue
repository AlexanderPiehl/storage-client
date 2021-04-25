<template>
  <v-app id="app">
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <div>
        <CardList :items="items" />
      </div>
    </v-main>
  </v-app>
</template>

<script>
import CardList from "@/components/CardList";

export default {
  name: "App",

  components: {
    CardList,
  },

  data: () => ({
    items: [
      {
        title: "Canon Kamera",
        subTitle: "20 Megapixel",
        description: "Super tolle Kameria mit vielen Funktionen.",
        photoUrl: "https://picsum.photos/200",
      },
      {
        title: "Sony Kamera",
        subTitle: "18 Megapixel",
        description:
          "Auch eine tolle Kamera, aber von einem anderem Hersteller.",
        photoUrl: "https://picsum.photos/200",
      },
      {
        title: "Mikrofon",
        subTitle: "Some specs",
        description: "Super Mikrofon für Aufnahmen.",
        photoUrl: "https://picsum.photos/200",
      },
      {
        title: "Mikrofon 2",
        subTitle: "Another Specs",
        description: "Wir haben vielen Mikrofone",
        photoUrl: "https://picsum.photos/200",
      },
    ],
  }),
};
</script>

<style lang="scss">
#app {
  width: 100%;
}
</style>