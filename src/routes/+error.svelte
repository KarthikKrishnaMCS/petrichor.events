<main>
    <div>
        {#each Array(12) as _}
            <h1>Something went wrong!</h1>
        {/each} 
    </div>
</main>
<style>
    main{
        display: grid;
        place-items: center;
        height: 100vh;
        font-size: 30px;
    }
    h1{
        width: 30rem;
        margin-inline: 0.5rem;
    }
    div{
        position: absolute;
        display: flex;
        animation: loop 2s linear infinite;
        border-width: 10px 0px 10px 0px;
        border-style: solid;
        border-color: white;
    }

    @keyframes loop{
        from{
            left: 0
        }
        to{
            left: -31rem;
        }
    }
</style>  