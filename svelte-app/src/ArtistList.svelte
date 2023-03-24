<script>
  export let artists;
</script>

<div class="row justify-content-center">
  <div class="col-11 col-md-7 col-lg-5">
    <div class="list-group">
      {#each artists as { name, src, reknown }}
        <div
          class="list-group-item d-flex w-100 list-group-item-action
            align-items-center"
        >
          <img class="rounded mr-3 d-block" {src} alt={`Photo of ${name}`} />
          <div class="description">
            <h4 class="mb-0">{name}</h4>
            <p class="text-muted mb-0">{reknown}</p>
          </div>
        </div>
      {:else}
        <p>No data</p>
      {/each}
    </div>
  </div>
</div>

<style>
  img {
    height: 80px;
  }

  h4 {
    font-size: 1rem;
  }

  p {
    font-size: 0.8em;
  }
  .description {
    padding: 5px;
  }
</style>
