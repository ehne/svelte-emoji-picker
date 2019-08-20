<script>
	export let emojis = ["✌️","😂","😝","😁","😱","👉","🙌","🍻","🔥","🌈","☀️","🎈","🌹","💄","🎀","⚽","🎾","🏁","😡","👿","🐻","🐶","🐬","🐟","🍀","👀","🚗","🍎","💝","💙","👌","❤","😍","😉","😓","😳","💪","💩","🍸","🔑","💖","🌟","🎉","🌺","🎶","👠","🏈","⚾","🏆","👽","💀","🐵","🐮","🐩","🐎","💣","👃","👂","🍓","💘","💜","👊","💋","😘","😜","😵","🙏","👋","🚽","💃","💎","🚀","🌙","🎁","⛄","🌊","⛵","🏀","🎱","💰","👶","👸","🐰","🐷","🐍","🐫","🔫","👄","🚲","🍉","💛","💚"]
    export let value = ''
    export let fontSize = '30px'
	import { createEventDispatcher } from 'svelte';

	const select = num => () => value += num;
	const clear  = () => value = '';
	
</script>

<style>
	.emoji {
		background-color: rgba(0,0,0,0);
		border: 0px;
		cursor: pointer;
	}
	.emoji:hover {
		background-color: rgba(150,150,150,0.2);
		transition: all 0.5s;
		
	}
</style>


<div class="panel" style="font-size: {fontSize}">
	{#each emojis as emoji}
		<button class="emoji" on:click={select(emoji)}>
			{emoji}
		</button>
		
	{/each}
</div>