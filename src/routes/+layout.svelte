<script>
</script>

<svelte:head>
    <style>
		@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@500&display=swap');

		* {
			padding: 0;
			margin: 0;
			font-family: 'Roboto', sans-serif;
			scrollbar-width: none;
			letter-spacing: 0.5px;
		}

		body {
			background: #1f1f1f;
		}

		::-webkit-scrollbar {
				width: 0;
		}
		
	</style>
</svelte:head>

<div class="app">
    <header>
        <a href="/"><img src="https://cdn.discordapp.com/attachments/756373435726168104/769299914332962886/krnlmain.png" alt=""></a>
        <nav>
            <div class="ul">
                <a href="/">Download</a>
                <a href="/doc">Documentation</a>
                <a href="https://discord.com/invite/6AGKKRaT4z">Discord</a>
                <a href="/faq">Faq</a>
            </div>
        </nav>
    </header>
    
    <slot/>
    <footer>
        Copyright © Krnl 2022
    </footer>
    
</div>

<style>

    .app {
        color: white;
    }
    header {
        position: sticky;
        top: 0;
        display: flex;
        padding-inline: 2rem;
        justify-content: space-between;
        align-items: center;
        color: white;
        height: 10vh;
        background: #000000b2;
    }

    a {
        text-decoration: none;
        color: white;
    }

    
    img {
        width: 64px;
        height: 60px;
        margin-left: 2rem;
    }

    .ul {
        display: flex;
    }

    nav a {
        padding: 1rem 2rem;
        margin: 1rem;
        background: #004974;
        border-radius: 10px;
        transition: 0.3s;
    }

    nav a:hover {
        background: #006494;
    }

    nav a:active {
        transform: scale(0.9);
    }


    footer {
        text-align: center;
    }
</style>