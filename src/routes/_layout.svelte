<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
</script>

<style lang="scss" global>
  @import "./style/mixins.scss";
  @import "./style/main.scss";
  main {
    position: relative;
    max-width: 56em;
    //background-color: white;
    padding: 2em;
    margin: 0 auto;
    box-sizing: border-box;
    @include bp(medium) {
      // background-color: #444;
    }
  }
</style>

<Nav {segment} />

<main>
  <slot />
</main>
