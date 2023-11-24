<script>
    import InfoTile from "$lib/InfoTile.svelte"
    const data = [
        {
            type: "info", 
            title: "Shao",
            value: ""
        }
    ]
    const types = {
        "info": InfoTile
    }
</script>

{#each data as tile}
    <svelte:component this={types[tile.type]} title={tile?.title} props={tile.value}/>
{/each}