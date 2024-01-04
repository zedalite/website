<script lang="ts">
  import type { PageData } from "./$types";

  export let data: PageData;
</script>

<div class="container mx-auto flex flex-col items-center gap-8 p-8">
  <h1 class="h1">
    <span class="bg-gradient-to-br from-blue-500 to-cyan-300 bg-clip-text text-transparent box-decoration-clone">
        Quote Your Friends App
    </span>
  </h1>
  <div class="flex gap-2">
    <a href="/projects" class="btn variant-ghost">
      <span class="material-symbols-outlined"> keyboard_backspace </span>
      <span>Browse</span>
    </a>
    <a href="https://zedalite.de/#/login" target="_blank" rel="noreferrer noopener" class="btn variant-ghost">
      <span>Launch</span>
      <span class="material-symbols-outlined"> rocket_launch </span>
    </a>
  </div>
  <p>
    Explanation
  </p>
</div>
