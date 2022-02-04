<template>
  <div class="creator-footer" v-html="downloadedFooter"></div>
</template>

<script setup lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data(){
    return {
      downloadedFooter:""
    }
  },
  async fetch() {
    this.downloadedFooter = await this.$axios.$get('https://raw.githubusercontent.com/SaviPrograms/SaviPrograms/main/footer.html');
  },
  fetchOnServer: true,
})
</script>

<style lang="scss">
.creator-footer {
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;

  width: 100%;
  height: 4rem;

  color: rgba(49, 49, 49, 0.986);

  font-family: "Poiret One", sans-serif;

  a{
    color: black;
    font-family: "Srisakdi", cursive;
  }
}
</style>
