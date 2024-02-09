<script lang="ts">
  import type { SvelteComponent } from "svelte";

  // @ts-ignore
  export let component: new (...args: any[]) => SvelteComponent = undefined;

  export let style: string | undefined = "";
</script>

<svelte:component this={component} {style} />
