<script lang="ts">
	import Card from "../Card.svelte";

	let currentCard: Flashcard = {
		tokiPona: "ijo",
		english: "thing, placeholder, object"
	}
</script>

<Card card="{currentCard}"/>