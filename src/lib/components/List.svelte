<script lang="ts">
    import {  ListBox, ListBoxItem } from '@skeletonlabs/skeleton';
    export let heading: String;
    let v: string[] = ['concerts'];
 

    </script>
    <div class="size-wrapper"> 
    <ListBox multiple class="card p-1 text-token">
        <ListBoxItem bind:group={v} name="medium" value="" class="fa-solid fa-skull text-xl w-full text-center">{heading}</ListBoxItem>
    </ListBox>
    </div>
    <style>
        .size-wrapper{
            width: 80vw;
         }
    </style>

