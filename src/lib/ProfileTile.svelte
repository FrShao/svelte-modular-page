<script>
    import Tile from "./Tile.svelte"
    export let title
    export let value
</script>

<Tile {title}>
    <div>
        {value}
    </div>
    <img src={value.picture.src} alt={value.picture.alt}/>
</Tile>