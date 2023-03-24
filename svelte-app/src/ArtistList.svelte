<script>
  export let artists;
</script>

{#each artists as { name, src, reknown }}
  <div
    class="list-group-item d-flex w-100 list-group-item-action align-items-center"
  >
    <img class="rounded nr-3 d-block" {src} alt={`Photo of ${name}`} />
    <h2 class="artist-name mb-0 text-primary">
      {name}
    </h2>
    <p class="artist-reknown text-muted mb-0">{reknown}</p>
  </div>
{/each}
