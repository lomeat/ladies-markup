<script>
  import LogoIcon from "./icons/logo.svg";
  import SearchIcon from "./icons/search.svg";
  import CartIcon from "./icons/cart.svg";
  import MenuIcon from "./icons/menu.svg";

  import Button from "./Button.svelte";
</script>

<div class="wrapper">
  <div class="back-blue-square" />
  <header>
    <div class="logo">
      <span>Ladies</span>
      <LogoIcon style="margin-left: 14px" width="26" />
    </div>

    <div class="header-other">
      <div class="search">
        <input placeholder="Search" />
        <div class="search-button">
          <Button>
            <SearchIcon width="20" />
          </Button>
        </div>
      </div>
      <div class="cart">
        <Button>
          <CartIcon width="28" />
        </Button>
      </div>
      <div>
        <Button class="menu">
          <MenuIcon width="20" />
        </Button>
      </div>
    </div>
  </header>
  <main>
    <div class="best-sellers" />
    <div class="accessories" />
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
