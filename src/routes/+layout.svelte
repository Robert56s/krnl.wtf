<svelte:head>
  <style>
    @import url("https://fonts.googleapis.com/css2?family=Roboto:wght@500&display=swap");

    * {
      padding: 0;
      margin: 0;
      font-family: "Roboto", sans-serif;
      scrollbar-width: none;
      letter-spacing: 0.5px;
    }

    body {
      background: #111;
    }

    ::-webkit-scrollbar {
      width: 0;
    }

    @media screen and (max-width: 1045px) {
      html {
        font-size: 14px;
      }
    }
    @media screen and (max-width: 810px) {
      html {
        font-size: 12px;
      }
    }
    @media screen and (max-width: 629px) {
      html {
        font-size: 10px;
      }
    }
    @media screen and (max-width: 535px) {
      html {
        font-size: 8px;
      }
    }
  </style>
</svelte:head>

<div class="app">
  <header>
    <a href="/"><img src="https://cdn.discordapp.com/attachments/756373435726168104/769299914332962886/krnlmain.png" alt=""/></a>
    <nav>
      <a href="/download" data-sveltekit-prefetch>Download</a>
      <a href="/key" data-sveltekit-prefetch>Krnl Key</a>
      <a href="/doc" data-sveltekit-prefetch>Documentation</a>
      <a href="/discord"data-sveltekit-prefetch>Discord</a>
      <a href="/faq" data-sveltekit-prefetch>Faq</a>
    </nav>
  </header>

  <slot />
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
    height: 5.3rem;
    background: #000000b2;
  }

  a {
    text-decoration: none;
    color: white;
    white-space: nowrap;
  }

  img {
    width: 4rem;
    height: 3.75rem;
    margin-left: 2rem;
  }

  nav {
    display: flex;
    margin-inline: 2rem;
    flex-flow: row wrap;
  }

  nav a {
    display: flex;
    padding: 1rem 2rem;
    margin-inline: 1rem;
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

  @media screen and (max-width: 1045px) {
    nav {
        justify-content: center;
    }
    nav a {
        padding: 1rem;
        margin: 1rem 0.5rem;
    }
  }
  @media screen and (max-width: 445px) {
    header {
        height: 10.6rem;
        position: static;
    }
    nav a {
      padding: 1.2rem 2rem;
      margin: 0.5rem 1rem;
      font-size: 10px;
    }

  }
  @media screen and (max-width: 386px) {
    header {
        height: 10.6rem;
        position: static;
    }
    nav a {
      padding: 1.2rem 2rem;
      margin: 0.5rem 1rem;
      font-size: 10px;
    }

    nav a {
        padding: 1rem;
        margin: 1rem 0.5rem;
        font-size: 10px;
    }

  }
</style>
