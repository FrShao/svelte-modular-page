<script>
    export let title;
</script>

<div class="tile">
    {#if title}
        <div class="tile-title">
            {title}
        </div>
    {/if}
    <div>
        <slot/>
    </div>
</div>

<style>
    .tile {
        padding: 10px;
        box-shadow: 0px 0px 15px -3px rgba(0,0,0,0.2);
        display: flex;
        flex-direction: column;
    }
    .tile-title {
        border-bottom: solid 2px rgba(0,0,0,0.2);
        height: 2em;
    }
</style>