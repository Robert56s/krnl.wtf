<svelte:head>
    <!-- Primary Meta Tags -->
    <title>Krnl - Download</title>
    <meta name="title" content="Krnl - Discord" />
    <meta
      name="description"
      content="Ask for help in our new discord!"
    />

    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website" />
    <meta property="og:url" content="https://krnl.pw/discord" />
    <meta property="og:title" content="Krnl - Discord" />
    <meta
      property="og:description"
      content="Ask for help in our new discord!"
    />
    <meta
      property="og:image"
      content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
    />

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image" />
    <meta property="twitter:url" content="https://krnl.pw/discord" />
    <meta property="twitter:title" content="Krnl - Discord" />
    <meta
      property="twitter:description"
      content="Ask for help in our new discord!"
    />
    <meta
      property="twitter:image"
      content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
    />
</svelte:head>

<script>
    import { onMount } from "svelte";
    let a
    onMount(async () => {
        a.click()
    })
</script>
<!-- svelte-ignore a11y-missing-content -->
<a href="https://discord.com/invite/6AGKKRaT4z" style="display: none;" bind:this={a}  target="_blank" rel="noreferrer"></a>