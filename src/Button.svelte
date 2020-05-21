<script>
  export let className;
  export let active;
  export { className as class };
</script>

<button on:click class={className} class:active>
  <slot />
</button>

<style lang="scss">
  button {
    border: 0;
    margin: 0;
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

  .active {
    background: $bg-button-active;
    box-shadow: none;
  }

  .shadow {
    box-shadow: 0px 20px 20px $shadow-color;
  }

  .filter {
    padding: 28px 24px;
  }

  .menu {
    padding: 26px;
    background: $bg-card;
  }

  .arrow {
    border: 1px solid #e7e7e7;
  }

  .deactive {
    border: none;

    &:hover {
      background: $bg-button;
    }

    &:active {
      background: $bg-button;
    }
  }
</style>
