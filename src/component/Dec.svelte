<script lang="ts">
    import count from "../store/store";
  
      function dec() {
          count.update((v) => { return v -= 1})
      }
  </script>
  <button on:click={dec}>-</button>