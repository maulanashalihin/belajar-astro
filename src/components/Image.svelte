<script> 
    export let src="https://dripsender.id/wp-content/uploads/2023/02/testi1.jpg"
    import { scale } from 'svelte/transition';
    import { onMount} from 'svelte';
    export let alt;
    
    let visible = false; 



	onMount(() => {
		visible = true;
	});

</script>  
{#if visible}
<img  class="h-auto max-w-full" {alt} transition:scale={{ delay : 1000,  duration: 1000 }} src="{src}"  >
{:else}
<div class="invisible  h-48  ">
    .
    </div>
{/if}
 