<script>
  import Info from '../../_common/svelte/components/Info.svelte';
  import FeatureList from '../../_common/svelte/components/FeatureList.svelte';
  import Event from '../../_common/svelte/components/Event.svelte';
  import Binding from '../../_common/svelte/components/Binding.svelte';
  import Transition from '../../_common/svelte/components/Transition.svelte';
	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
  <Info first_name="Rich" last_name="Harris"/>
  <FeatureList/>
  <hr>
  <Event/>
  <hr>
  <Binding/>
  <hr>
  <Transition/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
