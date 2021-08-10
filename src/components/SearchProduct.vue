<template>
  <div>
    <input type="text" v-model="cari" placeholder="Cari Product">
    <ul>
      <li v-for="item in products" :key="item.id">
       {{ item.title }} , Harga : {{ item.price }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cari: '',
      products: [],
    };
  },
  created() {
    this.products = [
      {
        id: 1,
        title: "Product 1",
        price: 10000,
      },
      {
        id: 2,
        title: "Product 2",
        price: 20000,
      },
      {
        id: 3,
        title: "Product 3",
        price: 30000,
      },
      {
        id: 4,
        title: "Product 4",
        price: 40000,
      },
      {
        id: 5,
        title: "Product 5",
        price: 50000,
      },
    ];
  },
  computed:{
      cariData(){
          return this.products.filter((item) => {
              return item.title.match(this.cari)
          });
      }
  }
};
</script>
