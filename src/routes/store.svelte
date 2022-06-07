<script>
    let title = "Store!"
    import { fade } from "svelte/transition"
</script>

<svelte:head>
    <title>Store</title>
</svelte:head>

<div class="title-block">
    <h1 class="title" transition:fade>{title}</h1>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

    h1 {
        font-family: 'Pacifico', cursive;
        color: black;
        font-size: 42px;
    }

    .title-block {
        margin: 0px auto;
        width: 800px;
        display: flex;
        justify-content: center;
    }

</style>
