<script lang="ts">
    import count from "../store/store"
    let counter
    count.subscribe((v) => {
        counter = v
    })
</script>

<h1>{counter}</h1>