<script lang="ts">
  import { Avatar } from "@skeletonlabs/skeleton";
  import type { PageData } from "./$types";

  export let data: PageData;
</script>

<div class="container h-full mx-auto flex flex-col">
	<br/>
  <h1 class="h1 text-center">About Us</h1>
  <br/>
  <div class="flex gap-8 justify-center">
    <div class="flex flex-col items-center w-modal-slim card p-8 card-hover">
      <Avatar initials="JT" background="bg-primary-500" />
      <h2 class="h2">Jens</h2>
      <p>Co-Founder</p>
    </div>
    <div class="flex flex-col items-center w-modal-slim card p-8 card-hover">
      <Avatar initials="NK" background="bg-secondary-500" />
      <h2 class="h2">Niclas</h2>
      <p>Co-Founder</p>
    </div>
    <div class="flex flex-col items-center w-modal-slim card p-8 card-hover">
      <Avatar initials="SF" background="bg-tertiary-500" />
      <h2 class="h2">Simon</h2>
      <p>Developer</p>
    </div>
  </div>
</div>
