<template>
  <Navbar />
  <h1>UI Components</h1>
  <main>
    Hello
  </main>
</template>

<script>
import Navbar from './components/Navbar'
export default {
  name: 'App',
  components: {
    Navbar
  }
}
</script>

<style>
:root {
  --text-primary: #b6b6b6;
  --text-secondary: #ececec;
  --bg-primary: #202125;
  --bg-secondary: #141418;
  --transition-speed: 600ms;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
* {
  margin: 0;
  padding: 0;
}

body::-webkit-scrollbar {
  width: 0.50rem;
}

body::-webkit-scrollbar-track {
  background: #1e1e24;
}

body::-webkit-scrollbar-thumb {
  background: #6649b8;
}

main {
  margin-left: 5rem;
  padding: 1rem;
  margin-top: 5rem;
}

h1 {
  background: var(--bg-primary);
  margin-left: 5rem;
  padding: 1rem;
  height: 5rem;
  box-sizing: border-box;
  color: white;
  display: flex;
  align-items: center;
  font-weight: bold;
  text-transform: uppercase;
  font-size: 1.5rem;
  letter-spacing: 0.3ch;
  position: fixed;
  top: 0;
  width: 100%;
  box-shadow: 0 2px 5px 1px rgba(64,60,67,.16);
  z-index: 1;
}

/* Small Screens */
@media only screen and (max-width : 600px) {
  main {
    margin-left: 0;
  }

  h1 {
    margin-left: 0;
  }
}

</style>
