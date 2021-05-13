<template>
  <div>
    <topbar />
    <body-section style="margin-top:50px" />
  </div>
</template>

<script>
import topbar from "@/components/topbar.vue";
import bodySection from "@/components/body.vue";
export default {
  name: "Home",
  components: { topbar, bodySection },
};
</script>
