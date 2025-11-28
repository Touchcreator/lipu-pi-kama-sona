<script lang="ts">
	import { words } from "../words";
	import Card from "../Card.svelte";
	import Button from "../Button.svelte";

	let wordIndex = 0;

	function addWord() {
		if (wordIndex < words.length - 1) {
			wordIndex++;
		}
	}

	function minusWord() {
		if (wordIndex > 0) {
			wordIndex--;
		}
		
	}
</script>

<Card english={words[wordIndex].english} tokiPona={words[wordIndex].tokiPona}></Card>


<div class="self-center flex justify-center py-3">

    
    <Button text="&lt;" on:click={minusWord}/>

    <Button text="&gt;" on:click={addWord}/>

</div>
