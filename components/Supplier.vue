<template>
  <section>
    <div v-for="co in supplier" :key="co.id">
      <a href="co.location">
        <img :src="co.img" alt="" />
        <h3>{{ co.name }}</h3>
      </a>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      supplier: [
        {
          name: "ddfdf",
          img: "fgfgh",
          id: "hfuf7858",
          location: "gd"
        },
        {
          name: "ddfdf",
          img: "fgfgh",
          id: "hfuf7858",
          location: "gd"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped></style>
