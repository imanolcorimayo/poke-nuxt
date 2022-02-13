<template>
  <div>
    <div>{ span }</div>
    
    <div v-if="true"><Loading /></div>
    <div v-else><span>Holaa</span></div>
  </div>
</template>

<script>
import Loading from "../components/Loading";

export default {
  component: {
    Loading,
  },
};
</script>
