<script>
  let m = { x: 0, y: 0 };
  function handleMousemove(event) {
    m.x = event.clientX;
    m.y = event.clientY;
  }
  
  let status = true;
  function toggle() {
    status = !status;
  }
</script>
<style>
  div {
    width: 300px;
    height: 300px;
    margin: 0 auto;
    border: 1px solid #ff3e00;
  }
</style>
<h2>on:Event</h2>

<h3>click</h3>

{#if status}
  <button on:click={toggle}>
    click me..
  </button>
{:else}
  <button on:click={toggle}>
    Svelte - Cybernetically enhanced web apps
  </button>
{/if}

<h3>mousemove</h3>
<div on:mousemove={handleMousemove}>
  The mouse position is {m.x} x {m.y}
</div>
