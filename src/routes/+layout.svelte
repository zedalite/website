<script lang="ts">
  import Footer from "./Footer.svelte";

  import "../app.postcss";
  import type { LayoutData } from "./$types";
  import { AppBar, AppShell } from "@skeletonlabs/skeleton";
  import { LightSwitch } from "@skeletonlabs/skeleton";
  import Navbar from "./Navbar.svelte";

  export let data: LayoutData;
</script>

<AppShell>
  <svelte:fragment slot="pageHeader">
    <AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
      <svelte:fragment slot="lead">
        <h2 class="h2">
          <span class="bg-gradient-to-br from-blue-500 to-cyan-300 bg-clip-text text-transparent box-decoration-clone">
            Zedalite
          </span>
        </h2>
      </svelte:fragment>
      <Navbar />
      <svelte:fragment slot="trail"><LightSwitch /></svelte:fragment>
    </AppBar>
  </svelte:fragment>
  <slot />
  <svelte:fragment slot="pageFooter">
    <Footer />
  </svelte:fragment>
</AppShell>
