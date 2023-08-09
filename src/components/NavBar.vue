<script setup lang="ts">
//import HelloWorld from "./components/HelloWorld";

const menuItems = [
  { title: 'Carousel', path: '#carousel' },
  { title: 'Intro', path: '#intro' },
  { title: 'Future Link', path: '#' }
]
</script>

<template>
  <v-app-bar fixed>
    <v-toolbar-items>
      <v-btn flat v-for="item in menuItems" :key="item.title" :href="item.path">
        {{ item.title }}
      </v-btn>
    </v-toolbar-items>
  </v-app-bar>
</template>

<style scoped lang="scss">
:deep(.v-toolbar__content) {
  justify-content: center;
}
</style>
