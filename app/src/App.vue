<template>
  <div>
    <div class="titleBar">
      <img src="@/assets/logo.png" class="titleBarImage" />
      <span>SCRCPY+</span>
    </div>
    <router-view style="margin-top: 3em" />
  </div>
</template>

<style>
/* Material 3 Variables */
:root {
  --foreground: #8867c0;
  --midground: #25202d;
  --background: #1C1B1F;
}

.m3-btn {
  background-color: var(--foreground);
  margin: 0.5em;
  padding: 0.35em 0.75em;
  border-radius: 10em;
  border: none;
  outline: none;
  transition-duration: 0.25s;
}
.m3-btn:hover {
  filter: brightness(1.5);
}

.m3-card {
  background: var(--midground);
  border-radius: 1em;
  width: fit-content;
  padding: 0.5em 1em;
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
  background-color: var(--foreground);
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
  position: fixed;
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