<script>
  import { AppBar } from "@skeletonlabs/skeleton";
  import Icon from '@iconify/svelte';
  import { goto } from '$app/navigation';


</script>

<!-- <AppBar slotDefault="place-self-left" slotTrail="place-content-end inline md:hidden" background="bg-black">
	<svelte:fragment slot="lead">
        <div class="bg-gradient-to-br from-blue-500 to-cyan-300 bg-clip-text text-transparent box-decoration-clone text-2xl font-bold">
            Page Title
        </div>
    </svelte:fragment>
	
    <div class="flex flex-row items-center justify-end md:justify-between w-full">
        <div class="hidden md:inline">
            <button class="btn">Page 1</button>
            <button class="btn">Page 2</button>
            <button class="btn">Page 3</button>
        </div>
        <div>
            <button class="btn bg-cyan-600 font-bold rounded-lg">Sign In</button>
        </div>

    </div>

	<svelte:fragment slot="trail">
        <Icon icon="quill:hamburger" class="w-6 h-6"/>
    </svelte:fragment>
</AppBar> -->


<AppBar slotDefault="place-self-left" slotTrail="place-content-end inline md:hidden" background="bg-black">
	<svelte:fragment slot="lead">
        <div class="bg-gradient-to-br from-blue-500 to-cyan-300 bg-clip-text text-transparent box-decoration-clone text-2xl font-bold">
            Page Title
        </div>
    </svelte:fragment>
	
    <div class="flex flex-row items-center justify-end md:justify-between w-full">
        <div class="hidden md:inline">
            <button 
                class="btn" 
                on:click={() => {goto(`/`);}}
            >
                Home
            </button>
            <button 
                class="btn" 
                on:click={() => {goto(`/animation-test`);}}
            >
                Animation Test
            </button>
            <button class="btn">Page 3</button>
        </div>
        <div>
            <button class="btn bg-cyan-600 font-bold rounded-lg">Sign In</button>
        </div>

    </div>

	<svelte:fragment slot="trail">
        <Icon icon="quill:hamburger" class="w-6 h-6"/>
    </svelte:fragment>
</AppBar>