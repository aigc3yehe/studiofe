<script setup lang="ts">
import Chat from './components/Chat.vue'
</script>

<template>
  <n-message-provider>
    <Chat />
  </n-message-provider>
</template>

<style>
/* 重置默认样式 */
:root {
  --sl-color-gray-950: #131316;
  --sl-color-gray-900: #18181b;
  --sl-color-gray-800: #27272a;
  --sl-color-gray-700: #3f3f46;
  --sl-color-gray-600: #52525b;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body, #app {
  height: 100%;
  width: 100%;
  overflow: hidden;
}

#app {
  background-color: var(--sl-color-gray-950, #09090b);
}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
