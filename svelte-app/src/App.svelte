<script>
  import ArtistList from "./ArtistList.svelte";
  import ArtistSearch from "./ArtistSearch.svelte";
  let searchTerm = "Barot Bellingham";
</script>

<div class="container">
  <ArtistList {searchTerm} />
</div>

<style global lang="scss">
  $primary: purple;

  @import "../node_modules/bootstrap/scss/bootstrap.scss";
</style>
