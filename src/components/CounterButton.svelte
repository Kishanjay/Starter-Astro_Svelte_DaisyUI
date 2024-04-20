<script lang="ts">
  let clickCount: number = 0;

  function incrementClickCount() {
    clickCount += 1;
  }
</script>

<button class="btn" on:click={incrementClickCount}>
  Click me: {clickCount}!
</button>
