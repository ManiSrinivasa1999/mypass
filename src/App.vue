<template>
  <v-app>
    <v-navigation-drawer app>
      <!-- -->
    </v-navigation-drawer>

    <v-app-bar app>
      <!-- -->
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';
import { dom } from '@fortawesome/fontawesome-svg-core';

@Component({
  components: {},
})
export default class App extends Vue {
  // life-cycle hooks
  // Eg: mounted, created, destroyed
  mounted() {
    this.$nextTick(() => {
      dom.watch();
    });
  }

  // data

  // computed

  // methods

  // watchers
}
</script>

<style lang="scss"></style>
