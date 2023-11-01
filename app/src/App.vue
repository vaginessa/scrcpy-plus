<template>
  <div>
    <div class="titleBar">
      <img src="@/assets/logo.png" class="titleBarImage" />
      <span>SCRCPY+</span>
    </div>
    <router-view />
  </div>
</template>

<style>
/* Material 3 Variables */
:root {
  --background: #1C1B1F;
}
/* Material 3 Variables */

* {
  font-family: Arial, Helvetica, sans-serif;
  color: white;
}
html, body {
  margin: 0;
  background-color: #1c1b1f;
  overflow-x: hidden;
}
body::-webkit-scrollbar { width: 0.5em; }
body::-webkit-scrollbar-thumb {
  background-color: #8867c0;
  border-radius: 1em;
  -webkit-app-region: drag;
}
</style>

<style scoped>
.titleBar {
  -webkit-app-region: drag;
  color: white;
  width: 100%;
  padding: 0.5em;
  font-family: Arial, Helvetica, sans-serif;
  background: var(--background);
  position: sticky;
  top: 0;
  z-index: 1000;
  text-overflow: clip;
  user-select: none;
}
.centerTitleBar {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
}
.titleBarImage {
  height: 17px;
  transform: translateY(2px);
  margin-right: 0.5em;
}
</style>