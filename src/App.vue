<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style>
:root {
  --light-red: #c04c4b;
  --dark-red: #a0403f;
  --blue: #6ea4bb;
  --light-yellow: #f0dba5;
  --dark-yellow: #9b8754;
  --dark-yellow-opacity: #b9a060;
  --color-text: #e7e7e6;
  --color-text-secondary: #f6f6f6;
  --bg-color: #f2f2f2;
  --black: #464646;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  list-style: none;
  text-decoration: none;
}
html {
  font-size: 62.5%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
body {
  font-size: 2rem;
  background-color: var(--bg-color);
  color: var(--black);
}
input {
  outline: none;
}
</style>
