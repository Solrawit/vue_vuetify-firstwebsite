<template lang="">
    <v-app-bar :elevation="2">
        <template v-slot:prepend>
            <v-app-bar-nav-icon></v-app-bar-nav-icon>
        </template>
        <v-icon icon="$vuetify" size="small"></v-icon>
        <v-app-bar-title>SUPERFLY</v-app-bar-title>
        <v-btn
  color="primary"
  href="PageTodo.vue"
  class="d-flex align-center"
>
  <v-icon left>mdi-book-alert</v-icon>
  <span>Todo</span>
</v-btn>
        <v-btn value="recent">
    <v-icon>mdi-history</v-icon>

    <span>Recent</span>
  </v-btn>

  <v-btn value="favorites">
    <v-icon>mdi-heart</v-icon>

    <span>Favorites</span>
  </v-btn>

  <v-btn value="nearby">
    <v-icon>mdi-map-marker</v-icon>

    <span>Nearby</span>
  </v-btn>
    </v-app-bar>
    
        
    



    <!-- Footer -->
    <v-footer
    class="bg-indigo-lighten-1 text-center d-flex flex-column"
  >
    <div>
      <v-btn
        v-for="icon in icons"
        :key="icon"
        :icon="icon"
        class="mx-4"
        variant="text"
      ></v-btn>
    </div>

    <div class="pt-0">
      Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
    </div>

    <v-divider></v-divider>

    <div>
      {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
    </div>
  </v-footer>
</template>


<script>
export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
    name: 'HomePage'
}
</script>
<style lang="">
    
</style>