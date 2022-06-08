<script>
    let title = "Just welcome!"
    import { fade } from "svelte/transition"
    import axios from "axios"
    let name = ""
/*
    async function loadData(){
        try {
            const url = "https://my-first-express-app-675.herokuapp.com/"
            const res = await fetch(url)
            const data = await res.json()
            console.log(data)
        }catch(err){
            console.log("Error: ", err)
        }
    }
    loadData()
*/

    const putLogin = async () => {
        try {
            const url = "https://my-first-express-app-675.herokuapp.com/"
            const res = await axios.put(url, {
                headers: {},
                params: {test: false, name}
            })
            console.log(res)
        }catch(err){
            console.log("ERROR: ", err)
        }
    }

</script>

<svelte:head>
    <title>Project</title>
</svelte:head>

<div class="title-block">
    <h1 class="title" transition:fade>{title}</h1>
</div>

<input type="text" bind:value={name} placeholder="Username">
<button on:click={putLogin}>Login</button>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

    h1 {
        font-family: 'Pacifico', cursive;
        color: black;
        font-size: 42px;
    }

    .title-block {
        margin: 0px auto;
        width: 600px;
        display: flex;
        justify-content: center;
    }

</style>
