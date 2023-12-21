<script lang="ts">
    import { invoke } from "@tauri-apps/api/tauri"
  
    let username = "";
    let roomnumber = 0;
  

</script>

<div>
    <h1>HELooooooooo</h1>
    <form class="row">
        <input id="greet-input" placeholder="Enter a name..." bind:value={username} />
        <input id="greet-input" placeholder="Enter a name..." bind:value={roomnumber} />
        <button type="submit">Greet</button>
    </form>
</div>