<script setup lang="ts">
  import { defineCustomElement } from 'vue';
  import '@generic-components/components/switch.js';
  import '@generic-components/components/accordion.js';
  import 'https://unpkg.com/two-up-element@1';

  // customElements.define('generic-accordion', defineCustomElement(GenericAccordion));
</script>

<template>
  <generic-switch></generic-switch>

  <GenericAccordion selected="1">
    <button>Home</button>
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        <a href="/">eiusmod tempor</a> incididunt ut labore et dolore magna
        aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
        laboris nisi ut aliquip ex ea commodo consequat.
      </p>
    </div>

    <button>About</button>
    <div>
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
    </div>

    <button>Contact</button>
    <div>
      Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis
      suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur.
    </div>
  </GenericAccordion>

  <div class="demo">
    <two-up>
      <div class="light">
        <h1>The Light Side</h1>
      </div>
      <div class="dark">
        <h1>The Dark Side</h1>
      </div>
    </two-up>
  </div>

  <router-view />
</template>

<style>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
two-up {
  flex: 1;
}
.light,
.dark {
  text-align: center;
  padding: 10px 0 0;
}
.dark {
  background: #555;
  color: #ccc;
}
</style>
