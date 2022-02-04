<template>
  <div class="text-logo">
    <nobr><span class="f">F</span><span class="e">E</span></nobr
    ><wbr /><nobr><span class="t">T</span><span class="a">A</span></nobr>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({})
</script>

<style lang="scss">
.text-logo {
  text-align: center;

  font-size: 10rem;

  font-family: 'Source Sans Pro', sans-serif;
/*
  font-family: "Bungee Hairline", cursive;
  font-weight: 800; */
  line-height: 0.8em;

  margin-left: .25em;
  margin-right: .25em;

  text-shadow: var(--c-hero-txt) 0px 0px 1rem, var(--c-hero-txt) 0px 0px .6rem, var(--c-hero-txt) 0px 0px .3rem,
    2px 2px 2px rgba(206, 89, 55, 0);

  span {
    display: inline-block;
    color: var(--c-hero-txt);
  }

  .f {
    transform: scaleX(-1);
  }

  .a {
    transform: scaleY(-1);
  }
}
</style>
