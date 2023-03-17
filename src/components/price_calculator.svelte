<script>
    let base_price = 100;
    let number_users = 1;
</script>
<div>
   <input class="border px-3 py-2 " type="number" bind:value="{number_users}">
   <div>
    Harga : {base_price * number_users}
   </div>
</div>