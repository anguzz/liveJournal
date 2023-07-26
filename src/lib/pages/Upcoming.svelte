<script>
	import List from '$lib/components/List.svelte';
	import { concerts } from '$lib/utils/data2';
	
</script>

<div class="container h-full mx-auto flex justify-center items-center font-bold ">some bands i'm excited to see soon!  </div>

<div class="container h-full mx-auto flex justify-center items-center pt-4 pb-8">
	<div class="space-y-5">
		<ul>
			{#each concerts as concert}
				<li>
					<List heading={concert.heading}  />
				</li>
			{/each}
		</ul>
	</div>
</div>
