<template>
  <div>
    <searchFilter v-model="searchText" />
    <selectFilter :selectsource="OptionsOne" @change="selected = $event" />
    <AllProducts :productsdata="products" />
    <pre>{{ $data }}</pre>
  </div>
</template>

<script>
import searchFilter from "@/components/searchFilter.vue";
import selectFilter from "@/components/selectFilter.vue";
import AllProducts from "@/components/AllProducts.vue";

export default {
  components: {
    AllProducts,
    selectFilter,
    searchFilter
  },
  data() {
    return {
      selected: "",
      searchText: "",
      OptionsOne: ["tacos", "pizza", "dim sum"],
      products: [
        {
          id: "56ggx7g7s",
          name: "كوع",
          img: "hghghgh",
          deatils: "urtytdtd"
        },
        {
          id: "56ggx7g7s",
          name: "كوع",
          img: "hghghgh",
          deatils: "urtytdtd"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped></style>
