<script>
    async function getPokes()
    {
        let link = "https://pokeapi.co/api/v2/pokemon?offset=0";
        const res = await fetch(link);
		const text = await res.json();

		if (res.ok) {
            console.log(text);
			return text.results;
        }
    }

    var start = 0;
    var end = 10;
</script>

{#await getPokes()}
    
{:then data} 
{/await}