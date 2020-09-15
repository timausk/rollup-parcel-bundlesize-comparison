<script>
  export let first_name;
  export let last_name;

  $: fullname = first_name + " " + last_name;
</script>

<style>
  h2 {
    color: #ff3e00;
    font-size: 2em;
    font-weight: 100;
  }
</style>

<h2>Svelte is a free and open-source JavaScript framework written by {fullname}</h2>

<p>Svelte is a radical new approach to building user interfaces.
  Whereas traditional frameworks like React and Vue do the bulk of their work in the browser,
  Svelte shifts that work into a compile step that happens when you build your app.
</p>

<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>

