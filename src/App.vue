<template>
  <v-app>
    <v-main>
      <HelloWorld />
      <a href="" class="btn btn-primary" tabindex="-1" role="button" aria-disabled="true">ทดสอบปุ่ม</a>
      <ImageDetailComponent />
      <br />
      <HomePage />
      <br />
      <PageTodo/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import HomePage from "./components/HomePage.vue";
import ImageDetailComponent from "./components/ImageDetailComponent.vue";
import PageTodo from "./components/PageTodo.vue";

export default {

  name: "App",
  components: {
    HelloWorld,
    HomePage,
    ImageDetailComponent,
    PageTodo
  },

  data: () => ({
    //
  }),
};
</script>
