<script>
    import Card from "../ui/Card.svelte";
    export let fb = {};
    const handleDelete = (itemId) => {
        console.log(itemId);
    }

</script>

<Card>
    <div class="num-list">
        {fb.rating}
    </div>
    <button on:click={() => handleDelete(fb.id)} class="close-icon">X</button>
    <div class="content">{fb.text}</div>
</Card>

<style>
    .close-icon {
        position: absolute;
        cursor: pointer;
        color: white;
        padding: 1rem;
        top: -10px;
        right: -10px;
        border-radius: 50%;
        background-color: #64748b;
    }
    .num-list {
        position: absolute;
        padding: 0.5rem 1rem;
        top: 4px;
        left: 4px;
    }
</style>