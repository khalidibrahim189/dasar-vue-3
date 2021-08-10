<template>
  <div>
    <div v-if="products.length">
      <ul>
        <li v-for="item in products" :key="item.id">
          Nama Barang : {{ item.title }} , Harga : {{ item.price }}
        </li>
      </ul>
    </div>
    <div v-else>
        <p>Data tidak ditemukan</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [],
    };
  },
created(){
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
    ]
}

};
</script>
