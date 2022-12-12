<svelte:head>
  <!-- Primary Meta Tags -->
  <title>Krnl - Best Roblox Utility Tool</title>
  <meta name="title" content="Krnl  - Best Roblox Utility Tool" />
  <meta
    name="description"
    content="Krnl is a scripting tool with an easy-to-use graphical interface that makes it simple to build and run scripts."
  />

  <!-- Open Graph / Facebook -->
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://krnl.pw/" />
  <meta property="og:title" content="Krnl  - Best Roblox Utility Tool" />
  <meta
    property="og:description"
    content="Krnl is a scripting tool with an easy-to-use graphical interface that makes it simple to build and run scripts."
  />
  <meta
    property="og:image"
    content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
  />

  <!-- Twitter -->
  <meta property="twitter:card" content="summary_large_image" />
  <meta property="twitter:url" content="https://krnl.pw/" />
  <meta property="twitter:title" content="Krnl  - Best Roblox Utility Tool" />
  <meta
    property="twitter:description"
    content="Krnl is a scripting tool with an easy-to-use graphical interface that makes it simple to build and run scripts."
  />
  <meta
    property="twitter:image"
    content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
  />
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
  </style>
</svelte:head>

<div class="app">
  <header>
    <a href="/"><img src="https://cdn.discordapp.com/attachments/756373435726168104/769299914332962886/krnlmain.png" alt=""/></a>
    <nav>
      <a href="/download" data-sveltekit-prefetch>Download</a>
      <a href="https://direct-link.net/337368/krnl-key" target="”_blank”" data-sveltekit-prefetch>Krnl Key</a>
      <a href="/doc" data-sveltekit-prefetch>Documentation</a>
      <a href="https://discord.com/invite/6AGKKRaT4z" target="_blank" rel="noreferrer" data-sveltekit-prefetch>Discord</a>
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
    height: 10vh;
    background: #000000b2;
  }

  a {
    text-decoration: none;
    color: white;
    white-space: nowrap;
  }

  img {
    width: 64px;
    height: 60px;
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
  @media screen and (max-width: 810px) {
    header {
        height: 20vh;
        position: static;
    }
  }
  @media screen and (max-width: 600px) {
    header {
        height: 30vh;
    }
  }
</style>
