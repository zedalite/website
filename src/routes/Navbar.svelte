<script lang="ts">
  import { page } from "$app/stores";

  $: classesActive = (href: string) => {
    if(href==="/" && $page.url.pathname === "/"){
      console.log("outta here");
      return 'btn variant-filled-primary';
    }else if (href==="/"){
      return 'btn variant-filled-surface';
    }
    return ($page.url.pathname.substring(1).includes(href.substring(1)) ? 'btn variant-filled-primary' : 'btn variant-filled-surface');
  }

</script>

<nav class="btn-group variant-filled-surface p-2" >
  <a href="/" class="{classesActive("/")}" data-sveltekit-preload-data="hover">Home</a>
  <a href="/about" class="{classesActive("/about")}" data-sveltekit-preload-data="hover">About</a>
  <a href="/projects" class="{classesActive("/projects")}"data-sveltekit-preload-data="hover">Projects</a>
</nav>

<style>
  .active {
    color: black;
  }
</style>
