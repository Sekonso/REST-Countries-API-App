<template>
  <div :class="colorStore.colorMode">
    <router-view></router-view>
  </div>
</template>

<script>
// Components import
import { useColorStore } from "@/store/useColorStore";

export default {
  // Components
  name: "App",
  setup() {
    const colorStore = useColorStore();

    return { colorStore };
  },
};
</script>
