<script>
  export let login;
</script>

<style>
  .level:not(:last-child) {
    margin-bottom: 1rem;
  }
  .border {
    box-shadow: 0 2px 10px rgba(90, 97, 105, 0.12);
  }
  .is-fullheight {
    height: 100vh;
    background: #fff;
  }
  .main-content {
    margin: 1rem 1rem 0 1rem;
    padding: 1rem;
    background: #fff;
  }
  .profile {
    padding: 1rem;
  }
  .sidebar {
    padding-top: 1rem;
  }
  .vertical {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .button-text {
    font-size: 12pt;
  }
</style>

<div class="columns is-gapless">
  <div class="column is-2">
    <div class="box border is-fullheight">
      <article class="media profile">
        <div class="media-content">
          <div class="content has-text-centered">
            <figure class="image is-128x128">
              <img
                src="https://bulma.io/images/placeholders/128x128.png"
                alt="Image" />
            </figure>
            <p class="title">USERNAME</p>
            <p class="subtitle">FULL NAME</p>
          </div>
        </div>
      </article>
      <div class="field has-addons">
        <p class="control is-expanded">
          <button class="button vertical is-primary is-large is-fullwidth">
            <i class="las la-envelope" />
            <span class="button-text">Message</span>
          </button>
        </p>
        <p class="control is-expanded">
          <button class="button vertical is-primary is-large is-fullwidth">
            <i class="las la-tools" />
            <span class="button-text">Setting</span>
          </button>
        </p>
        <p class="control is-expanded">
          <button
            class="button vertical is-primary is-large is-fullwidth"
            on:click={() => (login = false)}>
            <i class="las la-sign-out-alt" />
            <span class="button-text">Logout</span>
          </button>
        </p>
      </div>
      <aside class="menu is-medium sidebar">
        <ul class="menu-list">
          <li>
            <a href="/">
              <span class="icon">
                <i class="las la-tachometer-alt" />
              </span>
              <span>Home</span>
            </a>
          </li>
          <li>
            <a href="/">
              <span class="icon">
                <i class="las la-user" />
              </span>
              <span>User</span>
            </a>
          </li>
        </ul>
      </aside>
    </div>
  </div>
  <div class="column">
    <div
      class="navbar is-white border"
      role="navigation"
      aria-label="main navigation">
      <div class="navbar-start">
        <button class="button is-white">
          <i class="las la-bars" />
        </button>
      </div>
      <div class="navbar-end">
        <div class="navbar-item">
          <h1 class="title has-text-primary">ARES DASHBOARD</h1>
        </div>
      </div>
    </div>
    <div class="box main-content">
      <nav class="level">
        <div class="level-left">
          <p class="title has-text-info">User Management</p>
        </div>
        <div class="level-right">
          <div class="level-item">
            <div class="buttons has-addons">
              <button class="button is-success">Details</button>
              <button class="button is-warning">Edit</button>
              <button class="button is-danger">Delete</button>
              <button class="button is-link">Print</button>
            </div>
          </div>
        </div>
      </nav>
      <table class="table is-fullwidth">
        <thead>
          <tr>
            <th>#</th>
            <th>Username</th>
            <th>Role</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td />
            <td />
            <td />
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</div>
