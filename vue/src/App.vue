<template>
  <div id="nav">
    <Header/>
    <div id="app-vue-aside">
      <Aside/>
      <router-view/>
    </div>
  </div>

</template>

<style>

</style>

<script>
import Header from "@/components/Header";
import Aside from "@/components/Aside";

export default {
  name: "Layout",
  components: {
    Header,
    Aside,
  }
}
</script>