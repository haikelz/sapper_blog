<script>
function toggle() {
	window.document.body.classList.toggle('dark-mode')
}
</script>
<a on:click={toggle}>
	<slot/>
</a>
<style>
	:global(body.dark-mode) button {
		background-color: #1f1f28;
		color: white;
	}
</style>
