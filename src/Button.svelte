<script>
  export let className;
  export { className as class };
</script>

<button on:click class={className}>
  <slot />
</button>

<style lang="scss">
  button {
    border: 0;
    border-radius: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: $bg-button;
    padding: 20px;
    transition: all 0.1s ease;

    &:hover {
      background: #eee;
    }

    &:active {
      background: #ccc;
    }
  }

  .menu {
    padding: 26px;
    background: $bg-card;
  }
</style>
