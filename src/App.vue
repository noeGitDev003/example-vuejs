<template>
  <div id="app">
    <px-loader v-if="showLoading"></px-loader>
    <px-header v-if="!showLoading"></px-header>
    <px-content v-if="!showLoading"></px-content>
    <px-partners v-if="!showLoading"></px-partners>
    <px-footer v-if="!showLoading"></px-footer>
  </div>
</template>

<script>
import PxLoader from "@/components/PxLoader";
import PxHeader from "@/components/PxHeader";
import PxContent from "@/components/PxContent";
import PxPartners from "@/components/PxPartners";
import PxFooter from "@/components/PxFooter.vue";

export default {
  name: "App",
  components: {
    PxLoader,
    PxHeader,
    PxContent,
    PxPartners,
    PxFooter
  },

  data () {
    return {
      showLoading: true
    }
  },

  methods: {
    changeModeLoading () {
      setTimeout(() => {this.showLoading = !this.showLoading;}, 1000);
    }
  },

  mounted () {
    this.changeModeLoading();
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
