<template>
<ProductsList class="center"></ProductsList>
</template>

<script>
import ProductsList from "@/components/ProductsList";
export default {
  name: 'App',
  components: {ProductsList},
}
</script>

<style lang="scss">
$widthSuite: 1200px;

.center {
  padding-left: calc(50% - #{$widthSuite} / 2);
  padding-right: calc(50% - #{$widthSuite} / 2);
}
</style>
