<script>
  let features = [
    {item: 'is not another Framework'},
    {item: 'code is compiled ahead of time'},
    {item: 'has NO virtual DOM'},
    {item: 'has baked in CSS scoping'},
    {item: 'is Easy to Learn'},
    {item: 'has a Clean templating syntax'},
    {item: 'apps are Blazing fast & Extremely small'},
    {item: 'is "Truly Reactive"'}
  ]
</script>
<style>
  ul {
    max-width: 295px;
    margin: 0 auto;
    text-align: left;
  }
</style>
<h1>Svelte ..</h1>
<ul>
  {#each features as {item}}
    <li>{item}</li>
  {/each}
</ul>
