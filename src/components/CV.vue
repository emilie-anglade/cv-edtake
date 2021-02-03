<template>
  <div class="cv-container">
    <div class="left-container">
      <p>cv content</p>
    </div>
    <div class="right-container">
      <p>cv content</p>
    </div>
  </div>
</template>

<style>
  .cv-container {
    background-color: antiquewhite;
    display: flex;
    width: 99vw;
    height: 99vh;
    margin: 0;
    padding: 0;
  }
  .left-container {
    flex: 2;
    background-color: brown;
    color: white;
  }
  .right-container {
    flex: 3;
  }
</style>