<template>
  <section>
    <div class="div1">
      <div class="center">
        <h1>مع انترناشيونال انديكس</h1>
        <h1>طلباتك في طريق اليك</h1>
      </div>
      <div class="center hi">
        <b-button pill variant="primary" size="lg">Button</b-button>
        <b-button pill variant="outline-secondary" size="lg">Button</b-button>
      </div>
    </div>
    <div></div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
section {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 1fr;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  justify-content: center;
  justify-items: center;
  align-items: center;
}
.hh {
  display: inline-flex;
}
</style>
