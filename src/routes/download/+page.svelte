<svelte:head>
    <!-- Primary Meta Tags -->
    <title>Krnl - Download</title>
    <meta name="title" content="Krnl - Download" />
    <meta
      name="description"
      content="Download Krnl Latest version and Legacy version."
    />

    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website" />
    <meta property="og:url" content="https://krnl.pw/download" />
    <meta property="og:title" content="Krnl - Download" />
    <meta
      property="og:description"
      content="Download Krnl Latest version and Legacy version."
    />
    <meta
      property="og:image"
      content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
    />

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image" />
    <meta property="twitter:url" content="https://krnl.pw/download" />
    <meta property="twitter:title" content="Krnl - Download" />
    <meta
      property="twitter:description"
      content="Download Krnl Latest version and Legacy version."
    />
    <meta
      property="twitter:image"
      content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
    />
</svelte:head>
<div class="first">
    <h1>
        Download Krnl
    </h1>
    <div class="flex">
        <div class="box">
            <h1>Latest version</h1>
            <p>
                Want the latest version of Krnl? The new user interface
                provides with all necessary functions to run scripts.
            </p>
            <div class="ul">
                <a href="https://k-storage.com/krnl_beta.exe">Download Krnl</a>
            </div>
        </div>
        <div class="box">
            <h1>Legacy version</h1>
            <p>
                Still a fan of the old UI? The old user interface
                contains all of the old functions you are used to!
            </p>
            <div class="ul">
                <a href="https://k-storage.com/krnl_bootstrapper.exe">Download Krnl Legacy</a>
            </div>
        </div>
    </div>
</div>

<div class="second">
    <h1>Alternative downloads</h1>
    <table>
        <tr>
          <th>Type</th>
          <th>Link</th>
        </tr>
        <tr>
          <td>Krnl API</td>
          <td><a href="https://k-storage.com/bootstrapper/files/KrnlAPI.dll">https://k-storage.com/bootstrapper/files/KrnlAPI.dll</a></td>
        </tr>
        <tr>
          <td>Krnl WeAreDevs</td>
          <td><a href="https://wearedevs.net/d/Krnl">https://wearedevs.net/d/Krnl</a></td>
        </tr>
      </table>
</div>
<footer>
    Copyright © Krnl 2022
</footer>

<style>
    p {
        color: rgb(153, 153, 153);
    }
    a {
        text-decoration: none;
        color: white;
    }
    .first {
        padding: 2rem
    }
    .first h1 {
        text-align: center;
        font-size: 300%;
        padding: 2rem;
    }
    .box h1 {
        font-size: xx-large;
        text-align: left;;
    }
    .flex {
        display: flex;
        justify-content: center;
        flex-flow: row wrap;
    }
    .box {
        display: flex;
        flex-direction: column;
        padding: 1rem;
        margin: 3rem;
        max-width: 32rem;
        min-width: 300px;
        border-radius: 20px;
        background: #0c0c0c;
        flex: 1
    }
    .box h1, p {
        padding: 1rem;
        margin: 1rem;
    }

    .ul{
        display: flex;
    }
    
    .ul a {
        padding: 1rem 2rem;
        margin: 1rem;
        background: #004974;
        border-radius: 10px;
        transition: 0.3s;
    }
    .ul a:hover {
        background: #006494;
    }
    .ul a:active {
        transform: scale(0.9);
    }

    .second {
        background: #070707;
    }
    .second h1 {
        font-size: 200%;
        text-align: center;
        padding: 2rem;
    }
    table, td, th {
        border: 3px solid rgb(141, 141, 141);
        border-radius: 5px;
        padding: 1rem;
        text-align: center;
    }
    th {
        background: #111;
    }
    table a {
        color: #006494;
    }
    table {
        position: relative;
        width: 50%;
        border-collapse: collapse;
        left: 50%;
        transform: translate(-50%)
    }

    footer {
        text-align: center;
        background: #070707;
        padding: 2rem;
        padding-top: 3rem;
    }
</style>