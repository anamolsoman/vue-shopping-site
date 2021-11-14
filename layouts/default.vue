<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" fixed app>
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar fixed app elevation="1" dark class="primary">
      <v-app-bar-nav-icon
        class="hidden-md-and-up"
        @click.stop="drawer = !drawer"
      />
      <v-spacer class="hidden-sm-and-down" />
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-btn class="ma-1 hidden-sm-and-down" to="/" text>Home</v-btn>
      <v-btn class="ma-1 hidden-sm-and-down" to="/products" text
        >Products</v-btn
      >

      <v-btn class="ma-1 hidden-sm-and-down" to="/testimonials" text
        >Testimonials</v-btn
      >

      <v-btn class="ma-1 hidden-sm-and-down" to="/about" text>About</v-btn>

      <v-btn class="ma-1 hidden-sm-and-down" to="/contact" text>Contact</v-btn>
      <v-spacer />
    </v-app-bar>
    <v-main class="backgound-color">
      <Nuxt />
    </v-main>

    <!-- <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer> -->
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Mobile Store',
    }
  },
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800;900&display=swap');
#app {
  margin: 0;
  font-size: 16px;
  font-family: 'Montserrat', sans-serif !important;
  font-weight: 400;
}
* {
  margin: 0;
  padding: 0;
  outline: none;
}
a {
  text-decoration: none !important;
}
.backgound-color {
  background-color: rgb(246, 249, 252);
}
</style>
