<script setup></script>

<template>
  <h1>You did it!</h1>
  <p>
    Visit
    <a href="https://vuejs.org/" target="_blank" rel="noopener">vuejs.org</a> to
    read the documentation
  </p>
  <div
    id="cookie-declaration-container"
    style="border: 1px solid red; padding: 10px; margin: 10px"
  >
    <h2>Cookie Declaration</h2>
  </div>
</template>

<script setup>
import { onMounted } from "vue";
onMounted(() => {
  const el = document.createElement("script");
  el.id = "CookieDeclaration";
  el.src =
    "https://consent.cookiebot.com/51fc488e-8bf3-462e-92f5-f0f46a8500fc/cd.js";
  el.async = true;
  document.getElementById("cookie-declaration-container").appendChild(el);
});
</script>
