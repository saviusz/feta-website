<template>
  <section>
    <slot />
  </section>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="scss" scoped>
section {
  min-height: 4em;
  padding: 1em 2em;
  background-color: var(--c-bg);
  color: var(--c-txt);

  font-size: 1.1em;

  p {
    /* font-family: 'Baloo Chettan 2', cursive;
    font-family: 'Poiret One', cursive; */
    font-family: 'Sulphur Point', sans-serif;

    margin: 1em 0;

  }

  blockquote {

    /* font-family: 'Marck Script', cursive; */
    font-family: 'Moon Dance', cursive;
    /* font-family: 'Oooh Baby', cursive; */

    font-size: 1.6em;

    margin: .75em 0;

    border-left: solid .08em;

    padding: .25em 0 .25em .5em;

  }

  blockquote::before {
    content: open-quote;
  }

  blockquote::after {
    content: close-quote;
  }

  h1 {
    font-family: 'Ruda', cursive;
    font-size: 1.5em;

    text-decoration: underline solid .13em;
    text-underline-offset: .25em;

    margin-top: .5em;
  }
}
</style>
