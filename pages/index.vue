<template>
  <MainLayout>
    <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
      <div
        v-if="products"
        class="grid 2xl:grid-cols-5 lg:grid-cols-4 sm:grid-cols-3 grid-cols-1 gap-4"
      >
        <div v-for="product in products" :key="product">
          <ProductComponent :product="product" />
        </div>
      </div>
    </div>
  </MainLayout>
</template>

<script setup>
import MainLayout from "../layouts/MainLayout.vue";

const products = [
  {
    id: 1,
    title: "Product 1",
    description: "This is a description",
    url: "https://picsum.photos/id/212/800/800",
    price: 29.99,
  },
  {
    id: 2,
    title: "Product 2",
    description: "This is a description",
    url: "https://picsum.photos/id/213/800/800",
    price: 39.99,
  },
  {
    id: 3,
    title: "Product 3",
    description: "This is a description",
    url: "https://picsum.photos/id/214/800/800",
    price: 49.99,
  },
  {
    id: 4,
    title: "Product 4",
    description: "This is a description",
    url: "https://picsum.photos/id/215/800/800",
    price: 59.99,
  },
  {
    id: 5,
    title: "Product 5",
    description: "This is a description",
    url: "https://picsum.photos/id/216/800/800",
    price: 69.99,
  },
  {
    id: 6,
    title: "Product 6",
    description: "This is a description",
    url: "https://picsum.photos/id/217/800/800",
    price: 79.99,
  },
  {
    id: 7,
    title: "Product 7",
    description: "This is a description",
    url: "https://picsum.photos/id/218/800/800",
    price: 89.99,
  },
  {
    id: 8,
    title: "Product 8",
    description: "This is a description",
    url: "https://picsum.photos/id/219/800/800",
    price: 99.99,
  },
  {
    id: 9,
    title: "Product 9",
    description: "This is a description",
    url: "https://picsum.photos/id/220/800/800",
    price: 109.99,
  },
  {
    id: 10,
    title: "Product 10",
    description: "This is a description",
    url: "https://picsum.photos/id/221/800/800",
    price: 119.99,
  },
  {
    id: 11,
    title: "Product 11",
    description: "This is a description",
    url: "https://picsum.photos/id/222/800/800",
    price: 129.99,
  },
];

// let products = ref(null);
// onBeforeMount(async () => {
//   products.value = await useFetch("/api/prisma/get-all-products");
//   setTimeout(() => (userStore.isLoading = false), 1000);
// });
</script>
