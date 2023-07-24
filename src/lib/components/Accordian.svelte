<script lang="ts">
import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
export let heading: String;
export let content: String;
</script>
<div class="size-wrapper"> 
<Accordion  class="card p-1 text-token">
    <AccordionItem>
        <svelte:fragment slot="lead"><i class="fa-solid fa-skull text-xl w-6 text-center" /></svelte:fragment>
        <svelte:fragment slot="summary"><p class="font-semibold">{heading}</p></svelte:fragment>
        <svelte:fragment slot="content">
            <!-- prettier-ignore -->
            <p>
        {content}
            </p>
        </svelte:fragment>
    </AccordionItem>
  
</Accordion>
</div>
<style>
    .size-wrapper{
        width: 80vw;
     }
</style>