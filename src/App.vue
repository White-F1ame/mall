<template>
  <div id="nav">
    <Header/>
    <div id="app-vue-aside">
      <Aside/>
    </div>
  </div>
  <router-view/>
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