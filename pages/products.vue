<template>
  <div>
    <v-layout justify-center class="mt-4">
      <!-- <v-flex md2 lg2 class="hidden-sm-and-down">
        <v-card>
          <v-list v-for="category in categories" :key="category.id">
            <v-list-item>
              {{ category.name }}
            </v-list-item>
          </v-list></v-card
        >
      </v-flex> -->
      <v-flex md6 lg6 sm12 xs12>
        <v-layout wrap justify-space-between>
          <v-flex
            v-for="item in items"
            :key="item.id"
            md4
            lg3
            sm6
            xs6
            class="pa-1"
          >
            <v-card elevation="0" rounded="true" outlined>
              <v-card-title class="pa-0">
                <v-chip class="ma-2" color="green white--text"> 50% Off</v-chip>
                <v-img :src="item.img_url" class="product-image"></v-img>
              </v-card-title>
              <v-card-text class="pb-1">
                <h3 class="pb-1">{{ item.name }}</h3>
                <h4 class="d-block green--text">
                  ${{ item.rate_amount }} &nbsp;
                  <strike class="red--text">${{ item.display_amount }}</strike>
                </h4>
                <!-- <h4 class="green--text">${{ item.display_amount }}</h4> -->
              </v-card-text>
              <v-card-actions>
                <v-btn class="mx-2" small dark color="primary">
                  <v-icon dark> mdi-plus </v-icon>
                </v-btn></v-card-actions
              >
            </v-card></v-flex
          ></v-layout
        >
      </v-flex>
    </v-layout>
  </div>
</template>
<script>
export default {
  data() {
    return {
      categories: [
        {
          id: 1,
          name: 'Apple',
        },
        { id: 2, name: 'Samsung' },
        { id: 3, name: 'Sonata' },
      ],
      items: [
        {
          id: 1,
          name: 'Apple Watch',
          category: 'Watch',
          category_id: '1',
          img_url: require('@/static/img/products/1.jpg'),
          rate_amount: '150',
          display_amount: '250',
        },
        {
          id: 1,
          name: 'Apple Watch',
          category: 'Watch',
          category_id: '1',
          img_url: require('@/static/img/products/2.jpg'),
          rate_amount: '150',
          display_amount: '250',
        },
        {
          id: 1,
          name: 'Apple Watch',
          category: 'Watch',
          category_id: '1',
          img_url: require('@/static/img/products/3.jpg'),
          rate_amount: '150',
          display_amount: '250',
        },
        {
          id: 1,
          name: 'Apple Watch',
          category: 'Watch',
          category_id: '1',
          img_url: require('@/static/img/products/4.jpg'),
          rate_amount: '150',
          display_amount: '250',
        },
        {
          id: 1,
          name: 'Apple Watch',
          category: 'Watch',
          category_id: '1',
          img_url: require('@/static/img/products/5.jpg'),
          rate_amount: '150',
          display_amount: '250',
        },
      ],
    }
  },
}
</script>
<style scoped>
.product-image {
  margin: auto;
}
</style>
