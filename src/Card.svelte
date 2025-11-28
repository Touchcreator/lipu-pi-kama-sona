<script lang="ts">

    export let english: string;
    export let tokiPona: string;

    let turned = false;

    function flip() {
        if (turned) {
            turned = false;
        } else {
            turned = true;
        }
    }
</script>

<div class="flex justify-center w-full self-center">

	<button class="rounded-3xl bg-white space-y-4 h-60 w-100 flex justify-center items-center" on:click={flip}>
		<span class="text-center {!turned ? 'linja-pona text-9xl' : 'text-4xl'}">{turned ? english : tokiPona}</span>
	</button>

</div>