<script lang="ts">
  export let callback
</script>

<button on:click={callback}>
  GENERATE
</button>

<style lang="scss">
  button {
    padding: 1em 2em;
    background-color: rgba(255, 64, 0, 0.267);
    border-radius: 2em;
    border: 2px solid rgba(255, 62, 0, 0);
    outline: none;
    width: fit-content;
    cursor: pointer;
    color: currentColor;
    &:focus, &:hover {
      border: 2px solid #ff3e00;
    }

    &:active {
      background-color: rgba(255, 62, 0, 0.2);
    }
  }

  
</style>
