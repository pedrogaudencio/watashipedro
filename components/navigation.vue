<template>
  <header class="global-navigation">
    <nav class="global-navigation__menu">
      <ul>
        <li v-for="(item, index) in navItems" :key="index">
          <nuxt-link :to="item.path">
          {{ item.text }}
        </nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
  export default {
    data: function() {
      return {
        name: 'Navigation',
        navItems: [
          {path: '/projects', text: 'projects'},
          {path: '/timeline', text: 'timeline'},
          {path: '/life', text: 'life'},
          {path: '/contact', text: 'say hi'},
        ]
      }
    }
  }
</script>

<style scoped>
  .global-navigation {
    text-align: right;
    height: 70px;
    width: 100%;
    padding: 25px 20px;
    background: #000;
    margin-left: auto;
    margin-right: auto;
  }
  .global-navigation__menu {
    margin-top: auto;
    margin-bottom: auto;
  }
  ul {
    padding: 0;
  }
  ul > li {
    display: inline;
    padding-right: 30px;
  }
  a {
    color: #fff;
    text-decoration: none;
  }
</style>
