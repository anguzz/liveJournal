<script lang="ts">
  
    export let id: string;
    export let title: string = "";
    export let backgroundClass: string = "bg-neutral-200 dark:bg-neutral-900";
    export let textClass: string = "text-neutral-800 dark:text-neutral-200";
  </script>
  

  <div class="Footer {backgroundClass} {textClass}">
    <div class=" text-4xl text-center">{title}</div>
    <div >
      <slot />
    </div>
  </div>
  
  <style global>
    .page {
      min-height: calc(100vh - 4rem);
      width: 100%;
    }
  </style>