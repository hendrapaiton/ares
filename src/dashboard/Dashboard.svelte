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
        font-size: 10pt;
    }

    .is-warning {
        color: white;
    }
</style>

<div class="columns is-gapless">
    <div class="column is-2">
        <div class="box border is-fullheight">
            <article class="media profile">
                <div class="media-content">
                    <div class="content has-text-centered">
                        <figure class="image is-128x128">
                            <img src="https://bulma.io/images/placeholders/128x128.png" alt="Image"/>
                        </figure>
                        <p class="title is-5">USERNAME</p>
                        <p class="subtitle is-6">FULL NAME</p>
                    </div>
                </div>
            </article>
            <div class="field has-addons">
                <p class="control is-expanded">
                    <button class="button vertical is-primary is-large is-fullwidth">
                        <i class="las la-tools"/>
                        <span class="button-text">Setting</span>
                    </button>
                </p>
                <p class="control is-expanded">
                    <button class="button vertical is-primary is-large is-fullwidth" on:click={() => (login = false)}>
                        <i class="las la-sign-out-alt"/>
                        <span class="button-text">Logout</span>
                    </button>
                </p>
            </div>
            <aside class="menu is-medium sidebar">
                <ul class="menu-list">
                    <li>
                        <a href="/" class="is-active">
                            <span class="icon">
                                <i class="las la-user"/>
                            </span>
                            <span>User</span>
                        </a>
                    </li>
                </ul>
            </aside>
        </div>
    </div>
    <div class="column">
        <div class="navbar is-white border" role="navigation" aria-label="main navigation">
            <div class="navbar-start">
                <div class="navbar-item">
                    <button class="button is-white">
                        <i class="las la-bars"/>
                    </button>
                </div>
            </div>
            <div class="navbar-end">
                <div class="navbar-item">
                    <h1 class="title has-text-primary is-4">ARES DASHBOARD</h1>
                </div>
            </div>
        </div>
        <div class="box main-content">
            <nav class="level">
                <div class="level-left">
                    <p class="title has-text-info is-4">User Management</p>
                </div>
                <div class="level-right">
                    <div class="level-item">
                        <div class="buttons has-addons">
                            <button class="button is-success is-small">Add</button>
                            <button class="button is-warning is-small">Edit</button>
                            <button class="button is-danger is-small">Delete</button>
                            <button class="button is-link is-small">Print</button>
                        </div>
                    </div>
                </div>
            </nav>
            <table class="table is-fullwidth">
                <thead>
                <tr>
                    <th>#</th>
                    <th>Username</th>
                    <th>Full Name</th>
                    <th>Role</th>
                </tr>
                </thead>
                <tbody>
                <tr>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                </tr>
                </tbody>
            </table>
            <nav class="level">
                <div class="level-item">
                    <small class="is-size-7 has-text-grey has-text-centered">&copy; 2020
                        <a href="https://github.com/hendrapaiton">hendrapaiton</a>
                        all right reserved
                    </small>
                </div>
            </nav>
        </div>
    </div>
</div>
