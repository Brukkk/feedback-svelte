<script>
  import FeedbackItem from "./FeedbackItem.svelte";

    export let feedback = [];
</script>

{#each feedback as fb( fb.id )}
    <FeedbackItem {fb} />
{/each}