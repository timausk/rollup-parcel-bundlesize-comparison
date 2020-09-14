<script>
  import { fade, fly } from 'svelte/transition';
  let visible1 = true;
  let visible2 = true;
  let visible3 = true;
</script>

<style>
  div {
    display: flex;
    align-items: center;
    flex-direction: column;
    min-height: 100px;
  }
  
</style>

<h2>Transition</h2>

<div>
  <label>
    <input type="checkbox" bind:checked={visible1}>
    visible Text
  </label>
  {#if visible1}
    <p>Fades in and out</p>
  {/if}
</div>

<div>
  <label>
    <input type="checkbox" bind:checked={visible2}>
    fade Text
  </label>
  {#if visible2}
    <p transition:fade>Fades in and out</p>
  {/if}
</div>

<div>
  <label>
    <input type="checkbox" bind:checked={visible3}>
    fly Text
  </label>
  {#if visible3}
    <p transition:fly="{{ y: 200, duration: 2000 }}">
      Flies in and out
    </p>
  {/if}
</div>
