<template>
  <q-page class="">
    <metaverse />
    <Sponsors />
    <RecentUpdates />
  </q-page>
</template>

<script>
import Metaverse from "src/components/Metaverse.vue";
import RecentUpdates from "src/components/RecentUpdates.vue";
import Sponsors from "src/components/Sponsors.vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: { Metaverse, Sponsors, RecentUpdates },
  name: "IndexPage",
});
</script>
