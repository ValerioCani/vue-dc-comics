<template>
  <div id="app">
    <HeaderSection/>
    <MainSection/>
    <MidBand/>
    <FooterSection/>
  </div>
</template>

<script>
  import HeaderSection from './components/HeaderSection.vue';
  import MainSection from './components/MainSection.vue';
  import FooterSection from './components/FooterSection.vue';
import MidBand from './components/midBand.vue';

  export default {
    name: 'App',
    components: {
    HeaderSection,
    MainSection,
    FooterSection,
    MidBand
}
  }
</script>

<style lang="scss">
 @import './styles/general.scss';
 @import './styles/vars.scss';

</style>
