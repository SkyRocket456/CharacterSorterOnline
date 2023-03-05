<script lang="ts">
  let count: number = 0
  const increment = () => {
    count += 1
  }
</script>

<h1>New Page</h1>
<button on:click={increment}>
  count is {count}
</button>
