<template>
  <div>
    <Header />
    <div style="display:flex">
      <router-view />
    </div>
  </div>

</template>

<style>
</style>

<script lang="ts">

import Header from "@/components/Header.vue"
import Aside from "@/components/Aside.vue"

export default {
  name: "Layout",
  components: {
    Header,
    Aside,
  },
}
</script>
