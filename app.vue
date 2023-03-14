<script setup lang="ts">
  const { isDarkMode } = useDarkMode();
</script>

<template>
  <Body :style="isDarkMode ? 'background-color: black;' : ''"></Body>
  <div :style="isDarkMode ? { backgroundColor: 'black' } : ''">
    <Nav />
    <Heading />
    <Cards />
  </div>
</template>

<style>
  * {
    margin: 0;
    padding: 0;
    font-family: Oxygen, system-ui, -apple-system, BlinkMacSystemFont,
      'Segoe UI', Roboto, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue',
      sans-serif;
  }
</style>
