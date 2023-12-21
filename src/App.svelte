<script lang="ts">
  import Chat from './Pages/Chat.svelte';
  import Greet from './Pages/Greet.svelte'
  import { Router, Link, Route } from "svelte-routing";
  export let url = "";
</script>

<main class="container">

  <Router {url}>
    <nav>
      <Link to="/">Home</Link>
      <Link to="/chat">Chat</Link>
    </nav>
    <div>

      <Route path="/chat" component={Chat} />      
      <Route path="/" component={Greet} />

    </div>
  </Router>

</main>

<style>
  .logo.vite:hover {
    filter: drop-shadow(0 0 2em #747bff);
  }

  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00);
  }
</style>