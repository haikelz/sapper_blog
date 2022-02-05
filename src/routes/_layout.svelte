<script>
  import Header from '../components/Header.svelte';
  export let segment;
</script>

<style>
  .layout {
    display: flex;
    flex-direction: column;
    min-height: 100%;
    min-height: 100vh;
    font-family: 'Nunito', 'Poppins';
  }

  main {
    flex: 1;
    position: relative;
    margin: 0 auto;
    max-width: 1400px;
    padding: 1em 2em;
    box-sizing: border-box;
    width: 100%;
    display: flex;
    flex-direction: column;
    text-align: left;
    font-family: 'Nunito', 'Poppins';
  }

  footer {
    font-size: 1em;
    font-family: Rubik, sans-serif;
    margin: 1em auto;
    max-width: 1400px;
    padding: 2em 2em .4em 2em;
    text-align: center;
    width: 100%;
  }
</style>

<div class="layout">
  <Header {segment}/>

  <main>
    <slot></slot>
  </main>

  <footer>
    <span>
      &copy; 2020-{new Date().getFullYear()} Haikel.
      Powered by <a href="https://sapper.svelte.dev" target="_blank">Sapper</a>.
    </span>
  </footer>
</div>
