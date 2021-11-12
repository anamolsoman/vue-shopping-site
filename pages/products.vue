<template>
  <div>
    <v-layout justify-center>
      <v-flex md2 lg2>
        <v-card>
          <v-list v-for="category in categories" :key="category.id">
            <v-list-item>
              {{ category.name }}
            </v-list-item>
          </v-list></v-card
        >
      </v-flex>
      <v-flex md6 lg6 sm12 xs12>
        <v-layout wrap justify-space-between class="mt-4">
          <v-flex
            v-for="item in items"
            :key="item.id"
            md4
            lg3
            sm6
            xs6
            class="pa-1"
          >
            <v-card>
              <v-card-title class="pa-0">
                <v-img
                  :src="item.img_url"
                  class="product-image"
                  max-width="200px"
                ></v-img>
              </v-card-title>
              <v-card-text> <h3>watch</h3> </v-card-text>
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
          img_url: require('@/static/img/products/1.jpg'),
          rate_amount: '150',
          display_amount: '250',
        },
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
          img_url: require('@/static/img/products/1.jpg'),
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
