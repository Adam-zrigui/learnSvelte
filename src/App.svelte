<script lang="ts">
  import Patch from "./Patch.svelte";
  import PostList from "./PostList.svelte";
  import Dec from "./component/Dec.svelte";
  import Display from "./component/Display.svelte";
  import Inc from "./component/Inc.svelte";
  import Reset from "./component/Reset.svelte";
  let truthy = false
</script>

<main>
<button on:click={() => truthy= true}>
show component
</button>
{#if truthy}
   <Patch on:close={() => truthy = false} />
    <Inc />
    <Display />
    <Reset />
    <Dec />
{/if}
</main>
