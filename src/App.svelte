<script>
  export let name;
</script>

<style>
  i.las.la-plane-departure {
    margin: 0 !important;
    padding: 0 !important;
    font-size: 74pt;
  }
</style>

<section class="hero is-fullheight">
  <div class="hero-body has-text-centered">
    <div class="container">
      <h1 class="title is-size-1 has-text-primary">Hello {name}!</h1>
      <i class="las la-plane-departure has-text-danger" />
      <p class="subtitle is-size-5 has-text-warning">
        Visit the
        <a href="https://svelte.dev/tutorial">Svelte tutorial</a>
        to learn how to build Svelte apps
        <br />
        and
        <a href="https://bulma.io/documentation/">Bulma documentation</a>
        to learn how to layouting bulma.
      </p>
    </div>
  </div>
</section>
