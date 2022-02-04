<template>
  <div class="hero">
    <img src="http://feta.lo26.pl/gallery/zdj1.jpg" alt="" />
    <div class="img-overlay"></div>
    <div class="text">
      <h1><text-logo /></h1>
      <h2>Festiwal Ekspresji Twórców Amatorów</h2>
    </div>
    <font-awesome-icon icon="chevron-down" class="scroll_down" />
  </div>
</template>

<script setup lang="ts">
import Vue from 'vue'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import TextLogo from '~/components/index/text-logo.vue'
export default Vue.extend({
  components: {
    TextLogo,
    FontAwesomeIcon,
  },
})
</script>

<style scoped lang="scss">
.hero {
  width: 100%;
  height: 100vh;

  @media (orientation: portrait) {
    height: 60vh;
  }

  position: relative;

  -webkit-box-shadow: 0px 2px 13px 0px var(--c-shadow);
  -moz-box-shadow: 0px 2px 13px 0px var(--c-shadow);
  box-shadow: 0px 2px 13px 0px var(--c-shadow);

  > img {
    position: relative;
    width: 100%;
    height: 100%;

    object-fit: cover;
  }

  > .img-overlay {
    position: absolute;
    top: 0;
    left: 0;

    width: 100%;
    height: 100%;

    background-image: linear-gradient(rgba(0, 0, 0, 0.479));
    background-image: -webkit-gradient(
      linear,
      left top,
      left bottom,
      from(rgba(0, 0, 0, 0.479))
    );
  }

  > .text {
    position: absolute;
    left: 50%;
    top: 50%;

    transform: translate(-50%, -50%);

    display: flex;
    flex-flow: column nowrap;

    width: 100%;
    padding: 0 1.5rem;

    h2 {
      margin-top: 1em;
      text-align: center;
      font-size: 1.5em;
      letter-spacing: 0.125em;
      color: white;
      font-family: 'Poiret One', cursive;
      /* font-family: 'Srisakdi', cursive; */
    }
  }

  > .scroll_down {
    position: absolute;
    bottom: 1rem;
    left: 50%;
    transform: translateX(-50%);

    color: white;

    font-size: 3em;

    @media (orientation: portrait) {
      display: none;
    }

    animation: toBottomTranition 3s infinite ease-in-out;
  }

  @keyframes toBottomTranition {
    0% {
      opacity: 0%;
      transform: translate(-50%, -25%);
    }
    50% {
      opacity: 100%;
      transform: translate(-50%, 0%);
    }
    100% {
      opacity: 0%;
      transform: translate(-50%, 25%);
    }
  }
}
</style>
