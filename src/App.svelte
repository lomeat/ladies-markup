<script>
  import Button from "./Button.svelte";
  import Header from "./Header.svelte";
</script>

<div class="wrapper">
  <div class="back-blue-square" />
  <Header />
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
