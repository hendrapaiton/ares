<script>
  export let login;
</script>

<style>

</style>

<section class="hero is-light is-fullheight">
  <div class="hero-body">
    <div class="container">
      <div class="columns is-centered has-text-centered">
        <div class="column is-5-tablet is-4-desktop is-3-widescreen">
          <h1 class="title">Welcome!</h1>
          <form class="box">
            <div class="field">
              <div class="control">
                <input class="input" type="text" placeholder="Username" />
              </div>
            </div>
            <div class="field has-addons">
              <div class="control is-expanded">
                <input
                  class="input"
                  id="pass"
                  type="password"
                  placeholder="Password" />
              </div>
              <div class="control">
                <a href="/" class="button is-outlined">
                  <i class="las la-eye" />
                </a>
              </div>
            </div>
            <div class="field">
              <div class="control">
                <button
                  type="button"
                  class="button is-success is-fullwidth"
                  on:click|preventDefault={() => (login = true)}>
                  Login
                </button>
              </div>
            </div>
          </form>
          <small class="is-size-7 has-text-grey">
            &copy; 2020
            <a href="https://github.com/hendrapaiton">hendrapaiton</a>
            all right reserved
          </small>
        </div>
      </div>
    </div>
  </div>
</section>
