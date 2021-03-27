<template>
  <div>
    <input
      v-bind:value="search"
      v-on:input="$emit('input', $event.target.value)"
      id="name"
      type="search"
      placeholder="للبحث"
    />
  </div>
</template>

<script>
export default {
  props: {
    search: {
      type: String
    }
  }
};
</script>

<style lang="scss" scoped></style>
