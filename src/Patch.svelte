<script lang="ts">
  import { createEventDispatcher } from "svelte";

const disptach = createEventDispatcher()
</script>
<div class="">
    <h1>popus</h1>
    <button on:click={() => disptach('close')}>close</button>
</div>

<style></style>