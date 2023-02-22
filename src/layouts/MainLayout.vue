<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-dark text-white">
      <q-toolbar>
        <q-toolbar-title class="text-grey-4"> Logo Feo xd </q-toolbar-title>
        <q-list padding class="row col-7 justify-end gt-sm text-weight-bold">
          <q-item clickable v-ripple>
            <q-item-section class="text-grey-4"> Inicio </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section class="text-grey-4"> Restaurante </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section class="text-grey-4"> Paintball </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section class="text-grey-4">
              Sobre Nosotros
            </q-item-section>
          </q-item>

          <q-item clickable v-ripple>
            <q-item-section class="text-grey-4">
              <q-icon name="search" size="sm" />
            </q-item-section>
          </q-item>
        </q-list>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";

const linksList = [
  {
    title: "Github",
    caption: "github.com/quasarframework",
    icon: "code",
    link: "https://github.com/quasarframework",
  },
  {
    title: "Discord Chat Channel",
    caption: "chat.quasar.dev",
    icon: "chat",
    link: "https://chat.quasar.dev",
  },
  {
    title: "Forum",
    caption: "forum.quasar.dev",
    icon: "record_voice_over",
    link: "https://forum.quasar.dev",
  },
];

export default defineComponent({
  name: "MainLayout",

  components: {},

  setup() {
    const leftDrawerOpen = ref(false);

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
});
</script>
