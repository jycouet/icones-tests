<script>
  import { Icon, LibIcon } from "lib-icon";
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/npm/water.css@2/out/dark.css"
  />
</svelte:head>

<h1>App</h1>

{#each Object.entries(LibIcon) as [key, icon]}
  <center>
    <div>
      <Icon component={icon} style="width: 4rem; height: 4rem;" />
    </div>
    {key}
  </center>
{/each}
