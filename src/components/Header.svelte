<script>
  import Logo from './Logo.svelte'
  import Nav from './Nav.svelte'

  export let segment
</script>

<style>
  header {
    display: flex;
    margin: 0 auto;
    max-width: 1400px;
    padding: 0em 2em .3em 2em;
    width: 100%;
  }
</style>

<header>
  <Logo />
  <Nav {segment} />
</header>
