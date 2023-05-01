<script lang="ts">
    import count from "../store/store";
  
      function reset() {
          count.update((v) => v = 0)
      }
  </script>
  <button on:click={reset}>reset</button>