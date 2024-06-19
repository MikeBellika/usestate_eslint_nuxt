<script setup lang="ts">
const myState = useState<boolean>("state", () => false);
// This does not give any eslint errors
if (myState) {
  console.log("myState");
}
const myRef = ref(false);
// This gives an eslint error
if (myRef) {
  console.log("myRef");
}
</script>
<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
  </div>
</template>
