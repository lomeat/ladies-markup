<script>
  import Button from "./Button.svelte";
  import PlusIcon from "./icons/plus.svg";
  import PlusActive from "./icons/plusActive.svg";

  export let active;
</script>

<div class="card" class:active>
  <img src={`https://img.icons8.com/dusk/100/000000/document.png`} alt="card" />
  <div class="details">
    <h2 class="name">Face Mask</h2>
    <span class="name-second">Grape Fruit</span>
    <span class="price">$16.00</span>
    <div class="add">
      <Button class="shadow" {active}>
        {#if active}
          <PlusActive width="20" />
        {:else}
          <PlusIcon width="20" />
        {/if}
      </Button>
    </div>
  </div>
</div>

<style lang="scss">
  @import "./style/card";
</style>
