<script>
    let title = "Just welcome!"
</script>

<svelte:head>
    <title>Project</title>
</svelte:head>

<div class="title-block">
    <h1 class="title">{title}</h1>
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
