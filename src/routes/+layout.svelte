<script lang='ts'>
	// The ordering of these imports is critical to your app working properly
	
	
	//import '@skeletonlabs/skeleton/themes/theme-crimson.css';	
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { LightSwitch } from "@skeletonlabs/skeleton";
	import Footer from '$lib/pages/Footer.svelte';
</script>

<div class="p-3"> <LightSwitch /></div>
<slot />

