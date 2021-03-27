<template>
  <div>
    <select
      @change="$emit('change', $event.target.value)"
      :name="select"
      :id="select"
    >
      <option value>--Please choose--</option>
      <option v-for="option in selectsource" :key="option" :value="option">
        {{ option }}
      </option>
    </select>
  </div>
</template>

<script>
export default {
  props: {
    selectsource: {
      type: [Array, Object]
    },
    select: {
      type: String,
      default: "النوع"
    }
  }
};
</script>

<style lang="scss" scoped></style>
