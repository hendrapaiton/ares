<script>
  import Login from "./login/Login.svelte";
  import Dashboard from "./dashboard/Dashboard.svelte";
  let login = true;
</script>

{#if login}
  <Dashboard />
{:else}
  <Login />
{/if}
