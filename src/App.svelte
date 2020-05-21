<script>
  import Button from "./Button.svelte";
  import Header from "./Header.svelte";

  import FilterIcon from "./icons/filter.svg";
  import ArrowIcon from "./icons/arrow.svg";
  import ArrowDeactiveIcon from "./icons/arrowDeactive.svg";
</script>

<div class="wrapper">
  <div class="back-blue-square" />
  <Header />
  <main>
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
        <div class="card">
          <img
            src={`https://img.icons8.com/dusk/100/000000/document.png`}
            alt="card" />
        </div>
      </div>
    </div>
    <div class="acc" />
  </main>
</div>

<style lang="scss">
  :global(*) {
    box-sizing: border-box;
    outline: none;
    margin: 0;
    padding: 0;
  }

  :global(body) {
    margin: 0;
    padding: 16px;
    user-select: none;
    display: flex;
    width: 100vw;
    height: 100vh;
  }

  @import "./style/app";
</style>
