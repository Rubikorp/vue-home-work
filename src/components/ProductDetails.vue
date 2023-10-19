<template>
  <div class="product">
      <h1 class="product__name">{{product.name}}</h1>
      <p class="product__available">{{product.available ? 'Available' : 'Out of stock'}}</p>
      <p class="product__price">${{formattedPrice}}</p>
  </div>
</template>

<script>
export default {
  name: "ProductDetails",
  props: {
    product: Object,
  },
  data() {
    return {
      product: {
        name: this.product.name,
        available: this.product.available,
        price: this.product.price,
      }
    }
  },
  computed: {
    formattedPrice() {
      return `${this.product.price}`
    }
  }
}
</script>

<style scoped lang="scss">

</style>