<script>
  import ArtistList from "./ArtistList.svelte";
  import ArtistSearch from "./ArtistSearch.svelte";
  let searchTerm = "Barot Bellingham";
  let artists = [];
</script>

<div class="container">
  <ArtistSearch {searchTerm} />
  <ArtistList {artists} />
</div>

<style global lang="scss">
  $primary: purple;

  @import "../node_modules/bootstrap/scss/bootstrap.scss";
</style>
