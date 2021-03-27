<template>
  <section>
    <div v-for="product in productsdata" :key="product.id">
      <nuxt-link :to="`details/${product.id}`">
        <img :src="product.img" alt="" />
        <h3>{{ product.name }}</h3>
        <p>
          {{ product.deatils }}
        </p>
      </nuxt-link>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    productsdata: {
      type: [Array, Object]
    }
  }
};
</script>

<style lang="scss" scoped></style>
