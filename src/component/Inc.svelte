<script lang="ts">
  import count from "../store/store";

    function inc() {
        count.update((v) => v += 1)
    }
</script>
<button on:click={inc}>+</button>