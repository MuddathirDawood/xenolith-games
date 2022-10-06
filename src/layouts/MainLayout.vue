<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar class="primary-bg-color">
        <q-toolbar-title class="text-white text-center">
          Xenolith Games
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
      <q-page-sticky position="bottom-right" :offset="fabPos">
              <q-fab
                icon="ion-apps"
                direction="left"
                class="secondary-bg-color text-white"
                :disable="draggingFab"
                v-touch-pan.prevent.mouse="moveFab"
                external-label
              >
                <q-fab-action @click="onClick" external-label label-position="top" class="primary-bg-color text-white" icon="home" label="Home" :disable="draggingFab" to="/"/>
                <q-fab-action @click="onClick" external-label label-position="top" class="primary-bg-color text-white" icon="sports_esports" label="Games" :disable="draggingFab" to="/games" />
              </q-fab>
            </q-page-sticky>
    </q-page-container>

    <q-footer elevated>
        <q-toolbar class="primary-bg-color">
          <q-toolbar-title class="text-subtitle1 text-center">Copyright &copy; by Muddathir Dawood</q-toolbar-title>
        </q-toolbar>
      </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',

  setup () {
    const fabPos = ref([ 18, 18 ])
    const draggingFab = ref(false)

    return {
      fabPos,
      draggingFab,

      onClick () {
        // console.log('Clicked on a fab action')
      },

      moveFab (ev) {
        draggingFab.value = ev.isFirst !== true && ev.isFinal !== true

        fabPos.value = [
          fabPos.value[ 0 ] - ev.delta.x,
          fabPos.value[ 1 ] - ev.delta.y
        ]
      }
    }
  }
})
</script>

<style>

</style>
