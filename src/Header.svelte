<script>
  import LogoIcon from "./icons/logo.svg";
  import SearchIcon from "./icons/search.svg";
  import CartIcon from "./icons/cart.svg";
  import MenuIcon from "./icons/menu.svg";

  import Button from "./Button.svelte";
</script>

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


<style lang="scss">
  @import "./style/header";
</style>
