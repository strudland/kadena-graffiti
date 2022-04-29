<script>
    import Tile from './Tile.svelte';

    let dummyData = [0, 1, 2, 3, 4, 5, 6, 7];
</script>

<div class="graffiti-container">
    {#each dummyData as dummy}
        <Tile elementIndex={dummy} />
    {/each}
</div>

<style>
    .graffiti-container {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100%;
        background-color: cadetblue;
        overflow: scroll;
    }
</style>