<script>
	import Accordian from '$lib/components/Accordian.svelte';
	import { concerts } from '$lib/utils/data';
	import { LightSwitch } from '@skeletonlabs/skeleton';
</script>

<div class="container h-full mx-auto flex justify-center items-center font-bold ">some bands ive seen and thoughts on them!  </div>

<div class="container h-full mx-auto flex justify-center items-center pt-4 pb-8">
	<div class="space-y-5">
		<ul>
			{#each concerts as concert}
				<li>
					<Accordian heading={concert.heading} content={concert.content} />
				</li>
			{/each}
		</ul>
	</div>
</div>
