<script>
  import Login from "./login/Login.svelte";
  import Dashboard from "./dashboard/Dashboard.svelte";
  let login = false;
</script>

{#if login}
  <Dashboard bind:login={login} />
{:else}
  <Login bind:login={login} />
{/if}
