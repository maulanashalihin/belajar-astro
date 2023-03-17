<script>
    import {onMount} from "svelte" 
    export let src="https://dripsender.id/wp-content/uploads/2023/02/testi1.jpg"
    import { scale } from 'svelte/transition';
    
    let visible = false;
    onMount(()=>{
        visible = true;
    })
</script> 

{#if visible}
<img transition:scale={{  duration: 1000 }} src="{src}" alt="">
{:else}
<div class="invisible h-28 text-xs">
    .
    </div>
{/if}