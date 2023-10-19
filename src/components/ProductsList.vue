<template>
<ProductDetails v-for="item in products" :product="item"></ProductDetails>
</template>

<script>
import ProductDetails from "@/components/ProductDetails";
export default {
  name: "ProductsList",
  components: {ProductDetails},
  data() {
    return {
      products: [
        {
          name: "IphoneXR",
          available: true,
          price: 100.00,
        },
        {
          name: "Xiaomi Mi6",
          available: true,
          price: 190.00,
        },
        {
          name: "Samsung A6",
          available: false,
          price: 100.99,
        },
        {
          name: "Xiaomi 9 Pro",
          available: true,
          price: 130.00,
        },
        {
          name: "Zenko g2",
          available: false,
          price: 200.00,
        },
        {
          name: "Lenovo V6",
          available: true,
          price: 140.00,
        },
      ],
    }
  }

}
</script>

<style scoped lang="scss">

</style>