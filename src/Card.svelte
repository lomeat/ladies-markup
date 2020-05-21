<script>
  import Button from "./Button.svelte";
  import PlusIcon from "./icons/plus.svg";
</script>

<div class="card">
  <img src={`https://img.icons8.com/dusk/100/000000/document.png`} alt="card" />
  <div class="details">
    <h2 class="name">Face Mask</h2>
    <span class="name-second">Grape Fruit</span>
    <span class="price">$16.00</span>
    <div class="add">
      <Button class="shadow">
        <PlusIcon width="20" />
      </Button>
    </div>
  </div>
</div>

<style lang="scss">
  @import "./style/card";
</style>
