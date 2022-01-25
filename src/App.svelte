<script>
	import Button from "@smui/button";
	let message = 'hi';
</script>
<Button></Button>
<div>{message}</div>
<input id="message" type="text" bind:value={message}><br>
<button on:click={() => message='bye'}>say bye</button>