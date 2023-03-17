<script>
    import {onMount} from "svelte" 
    export let src="https://dripsender.id/wp-content/uploads/2023/02/testi1.jpg"
    import { scale } from 'svelte/transition';
    
    let visible = false;
    onMount(()=>{
        visible = true;
    })
</script> 
<div class="invisible text-xs">
.
</div>
{#if visible}
<img transition:scale={{ delay: 1000, duration: 1000 }} src="{src}" alt="">
{/if}