<script>
  import Far from 'svelte-fa';
  import { faMoon } from '@fortawesome/free-solid-svg-icons';
  import Dark from './Dark.svelte';
  export let segment;
</script>

<style>
  :global(body) {
		background-color: #E5E9F0;
		color: #2e3440;
		transition: background-color 0.3s;
	}
	:global(body.dark-mode) {
		background-color: #1F1F28;
		color: #E5E9F0;
	}

  nav {
    align-items: flex-end;
    display: flex;
    flex: 1;
    font-family: Rubik, sans-serif;
    font-weight: 500;
    justify-content: flex-end;
    text-transform: uppercase;
  }

  a {
    color: inherit;
    text-decoration: none;
    padding: 10px 5px;
    display: block;
    position: relative;
    margin-left: 20px;
  }

  a:not(.selected) {
    opacity: 0.7;
  }

  a::before {
    content: '';
    position: absolute;
    transition: transform .3s ease;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 2px;
    background: #AAA;
    transform: scaleX(0);
  }

  a:hover::before,
  .selected::before {
    transform: scaleX(1);
    background: blue;
  }

  .selected::before {
    background: #EBCB8B;
  }
</style>

<nav>
  <a class='{segment === "about" ? "selected" : ""}' href='about'>about</a>
  <a rel=prefetch class='{segment === "blog" ? "selected" : ""}' href='blog'>blog</a>
</nav>
