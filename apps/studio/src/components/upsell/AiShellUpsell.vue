<template>
  <upgrade-panel
    class="ai-shell-upsell"
    title="The SQL AI shell is not available yet"
    :description="description"
    :show-features="false"
    standalone
    wide
  >
    <ai-shell-preview v-if="false" />
  </upgrade-panel>
</template>

<script lang="ts">
import Vue from "vue";
import UpgradePanel from "./UpgradePanel.vue";
import AiShellPreview from "./AiShellPreview.vue";

export default Vue.extend({
  components: { UpgradePanel, AiShellPreview },
  data() {
    return {
      description:
        "AI features are coming to Lavabase soon.",
    };
  },
});
</script>
