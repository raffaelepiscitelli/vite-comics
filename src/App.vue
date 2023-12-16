<template lang="">
  <div>
    <AppHeader/>
    <JumbotronHeader/>
    <AppMain/>
    <AppFooter/>
  </div>
</template>
<script>
import AppHeader from './components/AppHeader.vue';
import JumbotronHeader from './components/JumbotronHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    JumbotronHeader,
    AppMain,
    AppFooter
  }
}
</script>
<style lang="scss">
@use './styles/general.scss' as *;

</style>
