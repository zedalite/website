<script lang="ts">
    import type { PageData } from './$types';
    import appIcon from '$lib/assets/adaptive_icon_template.svg';
    
    export let data: PageData;
</script>

<div class="container mx-auto flex justify-center gap-8 p-8">
    <a href="/projects/quote-your-friends" class="card bg-initial card-hover size-1/3">
        <header>
            <img src={appIcon} class="w-full" alt="App-Icon"/>
        </header>
        <div class="p-4">
            <h3 class="h3">Quote Your Friends</h3>
            <article>A app to share quotes between friends</article>
        </div>
    </a>
    <div class="card bg-initial card-hover size-1/3">
        <header>
            <!-- <img src={appIcon} class="w-full" alt="App-Icon"/> -->
        </header>
        <div class="p-4">
            <h3 class="h3">Coming...</h3>
            <article>The next project in development</article>
        </div>
    </div>
</div>


