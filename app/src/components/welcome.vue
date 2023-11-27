<template>
    <section>
        <img alt="scrcpy-plus logo" src="../assets/logo.png">
        <h1>SCRCPY+</h1>
        <div>{ Version }</div>
        <div class="m3-btn-group">
            <button>Changelog</button>
            <button>Info</button>
            <button>Wireless</button>
        </div>

    </section>
</template>

<style scoped>
img {
    max-width: 5em;
    margin-top: 2em;
}
h1 {
    margin: 0;
}

.m3-btn-group > button {
  background-color: var(--midground);
  margin: 0.25em;
  margin-top: 2em;
  padding: 1em;
  border: none;
  outline: none;
  height: 5em;
  width: 8em;
  transition-duration: 0.25s;
}
.m3-btn-group > button:hover {
  background-color: var(--foreground);
}
.m3-btn-group > button:first-child {
  border-radius: 1em 0 0 1em;
}
.m3-btn-group > button:last-child {
  border-radius: 0 1em 1em 0;
}
</style>