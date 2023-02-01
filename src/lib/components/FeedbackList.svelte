<script>
    import Card from "../ui/Card.svelte";
    export let feedback = [];
</script>

{#each feedback as fb( fb.id )}
    <li>{fb.text} <strong>{fb.rating}</strong></li>
    
{/each}