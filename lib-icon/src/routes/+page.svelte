<script>
  import { LibIcon } from "$lib";
  import Icon from "$lib/Icon.svelte";
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/npm/water.css@2/out/dark.css"
  />
</svelte:head>

<h1>Lib</h1>

{#each Object.entries(LibIcon) as [key, icon]}
  <center>
    <div>
      <Icon component={icon} style="width: 4rem; height: 4rem;" />
    </div>
    {key}
  </center>
{/each}

<center>
  <!-- A basic anchor icon from Phosphor icons -->
  <div class="i-ph-anchor-simple-thin" />
  <!-- An orange alarm from Material Design Icons -->
  <div class="i-mdi-alarm text-orange-400" />
  <!-- A large Vue logo -->
  <div class="i-logos-vue text-3xl" />
  <!-- Sun in light mode, Moon in dark mode, from Carbon -->
  <button class="i-carbon-sun dark:i-carbon-moon" />
  <!-- Twemoji of laugh, turns to tear on hovering -->
  <div
    class="i-twemoji-grinning-face-with-smiling-eyes hover:i-twemoji-face-with-tears-of-joy"
  />
</center>
