<script>
  export let artists;
</script>

{#each artists as artist}
  <div
    class="list-group-item d-flex w-100 list-group-item-action align-items-center"
  >
    <img
      class="rounded nr-3 d-block"
      src={artist.src}
      alt={`Photo of ${artist.name}`}
    />
    <h2 class="artist-name mb-0 text-primary">
      {artist.name}
    </h2>
    <p class="artist-reknown text-muted mb-0">{artist.reknown}</p>
  </div>
{/each}
