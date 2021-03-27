<template>
  <section>
    <nav>
      <ul>
        <li>
          <nuxt-link to="/"><Logo /></nuxt-link>
        </li>
      </ul>
      <ul class="menu">
        <li><nuxt-link to="/">الرئيسة</nuxt-link></li>
        <li><nuxt-link to="/product">المنتجات</nuxt-link></li>
      </ul>
    </nav>
  </section>
</template>

<script>
import Logo from "@/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style lang="scss" scoped>
nav {
  height: 75px;
  background: #ffff;
  color: black;
  position: relative;
  align-items: center;
  display: flex;
  justify-content: space-between;

  a {
    color: #ffffff;
    text-decoration: none;
  }

  ul {
    display: flex;
    align-items: center;
    list-style: none;
    width: 50%;
    padding: 0;
    margin: 0;

    li {
      padding-right: 40px;
    }
  }
  .menu {
    justify-content: flex-end;
    margin-left: 10%;

    li {
      background: #0195ff;
      transition: background ease 0.25s;
      border-radius: 20px;
      padding: 5px 20px;
      margin-left: 10px;
      text-decoration: none;
      cursor: pointer;
      text-align: center;
      color: #ffffff;
      -webkit-appearance: none;
      -moz-appearance: none;
    }
    li:hover {
      background: #008bf0;
    }
  }
}
</style>
