<script>
  import Button from "./Button.svelte";
  import Card from "./Card.svelte";

  import FilterIcon from "./icons/filter.svg";
  import ArrowIcon from "./icons/arrow.svg";
  import ArrowDeactiveIcon from "./icons/arrowDeactive.svg";
</script>

<div class="bs">
  <div class="bs-header">
    <h1 class="name">Best Sellers</h1>
    <div class="filter">
      <Button class="shadow filter">
        <FilterIcon width="22" />
      </Button>
    </div>
    <div class="arrows-wrapper">
      <div class="arrow arrow-left">
        <Button class="arrow">
          <ArrowIcon width="20" />
        </Button>
      </div>
      <div class="arrow arrow-right">
        <Button class="arrow deactive">
          <ArrowDeactiveIcon width="20" />
        </Button>
      </div>
    </div>
  </div>

  <div class="bs-list">
    <Card active />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
  </div>
</div>

<style lang="scss">
  @import "./style/best-sellers";
</style>
