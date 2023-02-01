<script>
    import Card from "../ui/Card.svelte";
    export let fb = {};

</script>

<Card>
    <div class="num-list">
        {fb.id}
    </div>
    <div class="close-icon">X</div>
    <div class="content">{fb.text}</div>
</Card>

<style>
    .close-icon {
        position: absolute;
        cursor: pointer;
        padding: 0.5rem 1rem;
        top: 0;
        right: 0;
    }
    .num-list {
        position: absolute;
        padding: 0.5rem 1rem;
        top: 0;
        left: 0;
    }
</style>