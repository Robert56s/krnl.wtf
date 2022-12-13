<svelte:head>
  <!-- Primary Meta Tags -->
  <title>Krnl - Documentation</title>
  <meta name="title" content="Krnl - Documentation" />
  <meta
    name="description"
    content="An official list of the Krnl environment, libraries, and other related information will be documented here. However, this documentation will not reflect on the active state of Krnl, and may be missing content. This will be updated regularly, any inconsistencies should be reported to Someone Papy#2062. Krnl is UNC supported to make scripting easier."
  />
  <!-- Open Graph / Facebook -->
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://krnl.pw/doc" />
  <meta property="og:title" content="Krnl - Documentation" />
  <meta
    property="og:description"
    content="An official list of the Krnl environment, libraries, and other related information will be documented here. However, this documentation will not reflect on the active state of Krnl, and may be missing content. This will be updated regularly, any inconsistencies should be reported to Someone Papy#2062. Krnl is UNC supported to make scripting easier."
  />
  <meta
    property="og:image"
    content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
  />
  <!-- Twitter -->
  <meta property="twitter:card" content="summary_large_image" />
  <meta property="twitter:url" content="https://krnl.pw/doc" />
  <meta property="twitter:title" content="Krnl - Documentation" />
  <meta
    property="twitter:description"
    content="An official list of the Krnl environment, libraries, and other related information will be documented here. However, this documentation will not reflect on the active state of Krnl, and may be missing content. This will be updated regularly, any inconsistencies should be reported to Someone Papy#2062. Krnl is UNC supported to make scripting easier."
  />
  <meta
    property="twitter:image"
    content="https://cdn.discordapp.com/attachments/828812665232425000/1051528825978241034/favicon1.png"
  />
</svelte:head>

<div class="body">
  <div>
    
    <div align="center" class="alertbanner">[Information] This is just a preview of what the documentation will look like. It is unfinished and information may be wrong.</div>
    
    <!-- Body -->
    <section style="height: 250px;">
      <div class="bodyhandler">
        <div style="margin-bottom: 50px;margin-top: 150px;" align="center">
          <h1 class="featuresinside" id="about">Documentation</h1>
        </div>
        <!-- Page size -->
        <div style="display: flex;height:3500px;">
          <div id="navt" class="leclas" style="width: 25%; position: fixed; height:80vh; margin-top:60px; top: 300px">
            <!-- Navigation -->
            <h1 align="center">Navigation</h1>
            <hr size="1" color="#282828" noshade="">
            <ul id="myUL">
              <li class="navitem"><a href="#information">General Information</a></li>
              <li class="navitem"><a href="#execenviron">Execution Environment</a></li>
              
<li class="navitem"><span class="caret navitem"><a href="#debug">debug</a></span>
<ul class="nested">
  <li class="navitem"><a href="#debug.getconstant">debug.getconstant</a></li>
  <li class="navitem"><a href="#debug.getconstants">debug.getconstants</a></li>
</ul>
</li>

<li class="navitem"><span class="caret navitem"><a href="#Drawing">Drawing</a></span>
<ul class="nested">
  <li class="navitem"><a href="#Drawing.new">Drawing.new</a></li>

<li class="navitem"><span class="caret navitem"><a href="#Drawing Types">Drawing Types</a></span>
<ul class="nested">
  <li class="navitem"><a href="#Image">Image</a></li>
  <li class="navitem"><a href="#Square">Square</a></li>
</ul>
</li>
</ul>
</li>

              <!-- Krnl API -->
              <li class="navitem"><a href="#krnlapi">Krnl API</a></li> <li class="navitem"><span class="caret navitem"><a href="#howtouse">Using The API</a></span> <ul class="nested"><li class="navitem"><a href="#krnlapiclass">KrnlAPI - Class</a></li> <li class="navitem"><a href="#initializeapi">Initialize</a></li> <li class="navitem"><a href="#injectapi">Inject</a></li> <li class="navitem"><a href="#executeapi">Execute</a></li></ul></li>
            </ul>
            <script>var i,toggler=document.getElementsByClassName("caret");for(i=0;i<toggler.length;i++)toggler[i].addEventListener("click",function(){this.parentElement.querySelector(".nested").classList.toggle("active"),this.classList.toggle("caret-down")});</script>
          </div>
          <!-- Documentation -->
          <div class="docs">
            <h1 align="center" id="information" class="headertext">Official KRNL Documentation</h1>
            <hr size="1" color="#282828" noshade="">
            <p class="desc">
              An official list of the Krnl environment, libraries, and other related information will be documented here.
              However, this documentation will not reflect on the active state of Krnl, and may be missing content.
              <br>
              <br>
              This will be updated regularly, any inconsistencies should be reported to <strong>Someone Insane#9501</strong>
              <br>

              <br>
              Krnl is UNC supported to make scripting easier.
              <br>
              <a href="https://scriptunc.org" style="height:max-content;" target="_blank" rel="noreferrer">
                <img style="width: 120px;height:auto;" alt="UNC Supported Badge" src="https://scriptunc.org/badge-supported.png"/>
              </a>
            </p>


            <h1 align="center" id="execenviron" class="headertext">Execution Environment</h1>
            <hr size="1" color="#282828" noshade="">
            <p class="desc">A reference to every function contained within the execution environment.</p>
            

<h1 align="center" id="debug" class="headeranchor">debug</h1>
<hr size="1" color="#282828" noshade="">

<div class="codesample">
<h3 id="debug.getconstant">debug.getconstant</h3><pre class="hljs">&lt;<span class="hljs-keyword">variant</span>&gt; <span class="hljs-built_in">debug</span>.<span class="hljs-built_in">getconstant</span>(union&lt;<span class="hljs-function"><span class="hljs-keyword">function</span>, <span class="hljs-title">int</span>&gt; <span class="hljs-title">fl</span>, &lt;<span class="hljs-title">int</span>&gt; <span class="hljs-title">index</span>)</span></pre>Returns the constant at the <strong>index</strong> of the function/level <strong>fl</strong><p><br><strong>EXAMPLE</strong></p><pre class="hljs"><span class="hljs-keyword">local</span> <span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">func</span><span class="hljs-params">(x)</span></span>
  <span class="hljs-built_in">print</span>(x, x == <span class="hljs-string">&quot;apple&quot;</span>)
<span class="hljs-keyword">end</span>

func(<span class="hljs-string">&quot;orange&quot;</span>) <span class="hljs-comment">--&gt; orange false</span>
func(<span class="hljs-built_in">getconstant</span>(func, <span class="hljs-number">1</span>)) <span class="hljs-comment">--&gt; apple true</span></pre>
</div>

<div class="codesample">
<h3 id="debug.getconstants">debug.getconstants</h3><pre class="hljs">&lt;<span class="hljs-built_in">table</span>&gt; <span class="hljs-built_in">debug</span>.<span class="hljs-built_in">getconstants</span>(union&lt;<span class="hljs-function"><span class="hljs-keyword">function</span>, <span class="hljs-title">int</span>&gt; <span class="hljs-title">fl</span>)</span></pre>Returns an array of all the constants of the function/level <strong>fl</strong><p><br><strong>EXAMPLE</strong></p><pre class="hljs"><span class="hljs-keyword">local</span> <span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">func</span><span class="hljs-params">(x)</span></span>
  <span class="hljs-built_in">print</span>(x, x == <span class="hljs-string">&quot;apple&quot;</span>)
<span class="hljs-keyword">end</span>

func(<span class="hljs-string">&quot;orange&quot;</span>) <span class="hljs-comment">--&gt; orange false</span>
func(<span class="hljs-built_in">getconstants</span>(func)[<span class="hljs-number">1</span>]) <span class="hljs-comment">--&gt; apple true</span></pre>
</div>


<h1 align="center" id="Drawing" class="headeranchor">Drawing</h1>
<hr size="1" color="#282828" noshade="">

<div class="codesample">
<h3 id="Drawing.new">Drawing.new</h3><pre class="hljs">&lt;<span class="hljs-built_in">table</span>&gt; <span class="hljs-built_in">Drawing</span>.new(&lt;<span class="hljs-built_in">string</span>&gt; <span class="hljs-built_in">type</span>)
  Properties:
  &lt;<span class="hljs-built_in">bool</span>&gt; Visible (<span class="hljs-literal">false</span>)
  &lt;<span class="hljs-built_in">number</span>&gt; Transparency (<span class="hljs-number">1</span>)
  &lt;<span class="hljs-built_in">int</span>&gt; ZIndex (<span class="hljs-number">0</span>)
  &lt;<span class="hljs-built_in">Color3</span>&gt; Color (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>, <span class="hljs-number">0</span>)

  Methods:
  &lt;<span class="hljs-built_in">void</span>&gt; Remove</pre>Creates a drawing object of the class <strong>type</strong><p><br><strong>EXAMPLE</strong></p><pre class="hljs"><span class="hljs-keyword">local</span> square = <span class="hljs-built_in">Drawing</span>.new(<span class="hljs-string">&quot;Square&quot;</span>)</pre>
</div>


<h1 align="center" id="Drawing Types" class="headeranchor">Drawing Types</h1>
<hr size="1" color="#282828" noshade="">

<div class="codesample">
<h3 id="Image">Image</h3><pre class="hljs">&lt;<span class="hljs-built_in">number</span>&gt; Rounding (<span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Size (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Position (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Color3</span>&gt; Color (<span class="hljs-number">1</span>, <span class="hljs-number">1</span>, <span class="hljs-number">1</span>)
writeonly&lt;<span class="hljs-built_in">string</span>&gt; Data (<span class="hljs-string">&quot;&quot;</span>)</pre>
</div>

<div class="codesample">
<h3 id="Square">Square</h3><pre class="hljs">&lt;<span class="hljs-built_in">bool</span>&gt; Filled (<span class="hljs-literal">false</span>)
&lt;<span class="hljs-built_in">number</span>&gt; Thickness (<span class="hljs-number">2</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Size (<span class="hljs-number">100</span>, <span class="hljs-number">100</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Position (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>)</pre>
</div>

            <!-- KRNL Api -->
            <h1 align="center" id="krnlapi" class="headertext">Krnl API</h1><hr size="1" color="#282828" noshade>
            <p class="desc">This is the documentation for the official Krnl API and how to use it. <br>The Krnl DLL is only designed for the official version of Roblox from their own site. Krnl will NOT inject into Roblox from the Microsoft Store, Linux or MacOs. <br><br>The API utilizes .NET Framework 4.8 (C#) <br><br> You can get the API <a style="color: rgb(100, 100, 200);" href="https://k-storage.com/bootstrapper/files/KrnlAPI.dll">here</a></p>

            <h1 align="center" id="howtouse" class="headertext">Using the API</h1>
            <h3 id="krnlapiclass">KrnlApi - class</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span> krnlApi = <span class="hljs-keyword" style="color: rgb(204, 153, 204);">new</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>(); </pre>
            <p class="compactDesc">This is the main class of the API which is used to access every function of the API. Create a new instance of this class to start using the API</p>

            <hr size="1" color="#282828" noshade>

            <h3 id="initializeapi">Initialize</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">void</span>> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.Initialize(); </pre>
            <p class="compactDesc">This method will set up the API and install all necessary files such as the DLL and only needs to be called one time. This method may cause a tiny bit of lag and should optimally be called when the application starts up. If lag is an issue, the API can be called through a thread.</p>

            <hr size="1" color="#282828" noshade>

            <h3 id="injectapi">Inject</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">void</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.Inject(); </pre>
            <p class="compactDesc">This method will inject the DLL into the active Roblox instance - keep in mind that the user has to go through the key system on their computer to gain unrestricted access to Krnl and the API.</p>

            <hr size="1" color="#282828" noshade>

            <h3 id="executeapi">Execute</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">bool</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.Execute(<span class="hljs-function"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">string</span> <span class="hljs-title" style="color: rgb(129, 162, 190);">script</span>); </pre>
            <p class="compactDesc">This method will execute the given script through the injected DLL. This will return true if the script has successfully been executed and false if there was a problem executing the script</p>

            <hr size="1" color="#282828" noshade>

            <h3 id="setframerate">SetFrameRate</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">void</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.SetFrameRate(<span class="hljs-function"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">int</span> <span class="hljs-title" style="color: rgb(129, 162, 190);">frameRate</span>); </pre>
            <p class="compactDesc">Sets the framerate of the active Roblox instance(s) to the desired value</p>

            <hr size="1" color="#282828" noshade>

            <h3 id="isinjectedapi">IsInjected</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">bool</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.IsInjected(); </pre>
            <p class="compactDesc">This method will check if the Krnl DLL has been injected</p>

            <hr size="1" color="#282828" noshade>

            <h3 id="isinitializedapi">IsInitialized</h3>
            <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"><span class="hljs-keyword" style="color: rgb(178, 148, 187);">bool</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.IsInitialized(); </pre>
            <p class="compactDesc">This method will check if the API has been initialized</p>
          </div>
        </div>
      </div>
      <!-- Footer -->
      <hr style="margin-top:600px;" size="1" color="#282828" noshade="">
      <div class="fatfuck">
        <p style="padding-bottom: 10px;" align="center">Copyright © Krnl 2022</p>
      </div>
    </section>
  </div>
</div>

<style>
  @font-face {
    font-family: 'Metropolis-SemiBold';
    src: local('Metropolis Semi Bold'), local('Metropolis-Semi-Bold'),
        url('Metropolis-SemiBold.woff2') format('woff2'),
        url('Metropolis-SemiBold.woff') format('woff'),
        url('Metropolis-SemiBold.ttf') format('truetype');
    font-weight: 600;
    font-style: normal;
}

@font-face {
    font-family: 'Metropolis-Medium';
    src: local('Metropolis Medium'), local('Metropolis-Medium'),
        url('Metropolis-Medium.woff2') format('woff2'),
        url('Metropolis-Medium.woff') format('woff'),
        url('Metropolis-Medium.ttf') format('truetype');
    font-weight: 500;
    font-style: normal;
}

@font-face {
    font-family: 'Metropolis-Bold';
    src: local('Metropolis Bold'), local('Metropolis-Bold'),
        url('Metropolis-Bold.woff2') format('woff2'),
        url('Metropolis-Bold.woff') format('woff'),
        url('Metropolis-Bold.ttf') format('truetype');
    font-weight: 700;
    font-style: normal;
}

.alertbanner
{
	background-color: #1f1c15;
	border-bottom-left-radius: 0px;
	border-bottom-right-radius: 0px;
	border-bottom-style: solid;
	border-bottom-width: 1px;
    border-left-style: solid;
    border-left-width: 0px;
    border-right-style: solid;
    border-right-width: 0px;
    border-top-color: rgb(277, 170, 65);
    border-top-left-radius: 0px;
    border-top-right-radius: 0px;
    border-top-style: none;
    border-top-width: 0px;
    box-sizing: border-box;
    color: rgb(227, 179, 65);
    display: block;
    font-size: 14px;
    font-weight: 600;
    line-height: 21px;
    margin-top: -1px;
    overflow-wrap: break-word;
    padding-bottom: 8px;
    padding-left: 16px;
    padding-right: 16px;
    padding-top: 8px;
    text-align: center;
    text-size-adjust: 100%;
}

.featuresinside {
    margin-bottom: 30px;
    margin-top: 30px;
    font-size: 35px;
    color: rgb(233, 233, 233);
}

.body {
    width: 100%;
    font-weight: normal;
    margin: 0;
    padding: 0;
    font-size: 16px;
    font-family: 'Metropolis-Medium', sans-serif;
    color: #8F8F9F;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    background: #171717;
}

.fatfuck {
    max-width: 100%;
    margin-left:15%;
    margin-right:15%;
}

.bodyhandler {
    max-width: 100%;
    margin-left:15%;
    margin-right:15%;
}

a {   
    border:none;
    outline:none;
    text-decoration:none;
    color:inherit; 
    transition:.2s ease;
}

a:hover {
    color: rgb(131, 131, 131);
}

h1 {
    font-size:30px;
}

h3{
    font-size:25px;
}

*, ::after, ::before {
    box-sizing: border-box;
}

ul, #myUL {
    list-style-type: none;
}
  
#myUL {
    margin-top: 20px;
    color: #DFDFDF;
    font-weight: 10;
}

.caret {
    cursor: pointer;
    -webkit-user-select: none; /* Safari 3.1+ */
    -moz-user-select: none; /* Firefox 2+ */
    -ms-user-select: none; /* IE 10+ */
    user-select: none;
    font-weight: 10;
}

.caret::before {
    content: "\25B8";
    color: gray;
    display: inline-block;
    margin-right: 6px;
}

.nested {
    display: none;
    transition: 300ms linear all;
    margin-top:10px;
}

.navitem {
    margin: 0 0 14px 0;
    font-family: "Lucida Sans Unicode", "Lucida Grande", sans-serif;
    font-size:14;
}

h1, h3 {
    color: #d5d5d5;
}

.headeranchor {
    padding-top: 50;
    margin-top: -50px;
}

.headertext {
    margin-top: 50px;
}

.desc {
    line-height: 150%;
    margin-bottom: 50px;
}

.compactDesc {
    line-height: 150%;
}

.codesample {
    margin-bottom: 55px;
}

.leclas {
    transition: visibility 0s, opacity 0.5s linear;
}

.docs {
    width: 60%;
    height:800px;
    margin-left:40%;
}

@media screen and (max-width: 1024px) 
{
    .leclas 
    {
        display: none !important;
    }

    .docs 
    {
        margin-left:0 !important;
        align-content: center !important;
        width:100%;
    }

    .bodyhandler 
    {
        margin-left:4%;
        margin-right:4%;
    }

    .featuresinside
    {
        visibility: hidden;
    }
}

/* Tomorrow Night Eighties Theme */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */

.hljs {
    background: #1d1f21;
    color: #c5c8c6;
    display: block;
    overflow-x: auto;
    padding: .5em;
  }
  
  /* Tomorrow Comment */
  .hljs-comment {
    color: #999999;
  }
  
  /* Tomorrow Orange */
  .hljs-number,
  .hljs-built_in,
  .hljs-literal,
  .hljs-params {
    color: #f99157;
  }
  
 
  
  /* Tomorrow Green */
  .hljs-string {
    color: #99cc99;
  }
  
  /* Tomorrow Blue */
  .hljs-title {
    color: #6699cc;
  }
  
  /* Tomorrow Purple */
  .hljs-keyword {
    color: #cc99cc;
  }

  .body {
    background-color: #111111;
  }
  h1 {
    padding: 1rem;
  }
</style>