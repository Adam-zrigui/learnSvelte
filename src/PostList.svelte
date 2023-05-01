<script lang="ts">
  import { onMount } from "svelte";
import axios from "axios"
    let posts = []
    onMount(async () => {
        const res = (await axios.get("https://jsonplaceholder.typicode.com/posts")).data
console.log(res)
posts = res
    })
</script>


<section>
    {#each posts as item (item.id)}
         <h3>{item.title}</h3>
    {/each}
</section>