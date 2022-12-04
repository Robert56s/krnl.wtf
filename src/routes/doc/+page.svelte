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
          <hr size="1" noshade="" color="#282828">
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
          <h1 id="information" class="headertext" align="center">Official KRNL Documentation</h1>
          <hr size="1" noshade="" color="#282828">
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
              <img style="width: 120px;height:auto;" alt="UNC Supported Badge" src="https://scriptunc.org/badge-supported.png">
            </a>
          </p>


          <h1 id="execenviron" class="headertext" align="center">Execution Environment</h1>
          <hr size="1" noshade="" color="#282828">
          <p class="desc">A reference to every function contained within the execution environment.</p>
          

<h1 id="debug" class="headeranchor" align="center">debug</h1>
<hr size="1" noshade="" color="#282828">

<div class="codesample">
<h3 id="debug.getconstant">debug.getconstant</h3><pre class="hljs">&lt;<span class="hljs-keyword">variant</span>&gt; <span class="hljs-built_in">debug</span>.<span class="hljs-built_in">getconstant</span>(union&lt;<span class="hljs-function"><span class="hljs-keyword">function</span>, <span class="hljs-title">int</span>&gt; <span class="hljs-title">fl</span>, &lt;<span class="hljs-title">int</span>&gt; <span class="hljs-title">index</span>)</span></pre>Returns the constant at the <strong>index</strong> of the function/level <strong>fl</strong><p><br><strong>EXAMPLE</strong></p><pre class="hljs"><span class="hljs-keyword">local</span> <span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">func</span><span class="hljs-params">(x)</span></span>
<span class="hljs-built_in">print</span>(x, x == <span class="hljs-string">"apple"</span>)
<span class="hljs-keyword">end</span>

func(<span class="hljs-string">"orange"</span>) <span class="hljs-comment">--&gt; orange false</span>
func(<span class="hljs-built_in">getconstant</span>(func, <span class="hljs-number">1</span>)) <span class="hljs-comment">--&gt; apple true</span></pre>
</div>

<div class="codesample">
<h3 id="debug.getconstants">debug.getconstants</h3><pre class="hljs">&lt;<span class="hljs-built_in">table</span>&gt; <span class="hljs-built_in">debug</span>.<span class="hljs-built_in">getconstants</span>(union&lt;<span class="hljs-function"><span class="hljs-keyword">function</span>, <span class="hljs-title">int</span>&gt; <span class="hljs-title">fl</span>)</span></pre>Returns an array of all the constants of the function/level <strong>fl</strong><p><br><strong>EXAMPLE</strong></p><pre class="hljs"><span class="hljs-keyword">local</span> <span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">func</span><span class="hljs-params">(x)</span></span>
<span class="hljs-built_in">print</span>(x, x == <span class="hljs-string">"apple"</span>)
<span class="hljs-keyword">end</span>

func(<span class="hljs-string">"orange"</span>) <span class="hljs-comment">--&gt; orange false</span>
func(<span class="hljs-built_in">getconstants</span>(func)[<span class="hljs-number">1</span>]) <span class="hljs-comment">--&gt; apple true</span></pre>
</div>


<h1 id="Drawing" class="headeranchor" align="center">Drawing</h1>
<hr size="1" noshade="" color="#282828">

<div class="codesample">
<h3 id="Drawing.new">Drawing.new</h3><pre class="hljs">&lt;<span class="hljs-built_in">table</span>&gt; <span class="hljs-built_in">Drawing</span>.new(&lt;<span class="hljs-built_in">string</span>&gt; <span class="hljs-built_in">type</span>)
Properties:
&lt;<span class="hljs-built_in">bool</span>&gt; Visible (<span class="hljs-literal">false</span>)
&lt;<span class="hljs-built_in">number</span>&gt; Transparency (<span class="hljs-number">1</span>)
&lt;<span class="hljs-built_in">int</span>&gt; ZIndex (<span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Color3</span>&gt; Color (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>, <span class="hljs-number">0</span>)

Methods:
&lt;<span class="hljs-built_in">void</span>&gt; Remove</pre>Creates a drawing object of the class <strong>type</strong><p><br><strong>EXAMPLE</strong></p><pre class="hljs"><span class="hljs-keyword">local</span> square = <span class="hljs-built_in">Drawing</span>.new(<span class="hljs-string">"Square"</span>)</pre>
</div>


<h1 id="Drawing Types" class="headeranchor" align="center">Drawing Types</h1>
<hr size="1" noshade="" color="#282828">

<div class="codesample">
<h3 id="Image">Image</h3><pre class="hljs">&lt;<span class="hljs-built_in">number</span>&gt; Rounding (<span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Size (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Position (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>)
&lt;<span class="hljs-built_in">Color3</span>&gt; Color (<span class="hljs-number">1</span>, <span class="hljs-number">1</span>, <span class="hljs-number">1</span>)
writeonly&lt;<span class="hljs-built_in">string</span>&gt; Data (<span class="hljs-string">""</span>)</pre>
</div>

<div class="codesample">
<h3 id="Square">Square</h3><pre class="hljs">&lt;<span class="hljs-built_in">bool</span>&gt; Filled (<span class="hljs-literal">false</span>)
&lt;<span class="hljs-built_in">number</span>&gt; Thickness (<span class="hljs-number">2</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Size (<span class="hljs-number">100</span>, <span class="hljs-number">100</span>)
&lt;<span class="hljs-built_in">Vector2</span>&gt; Position (<span class="hljs-number">0</span>, <span class="hljs-number">0</span>)</pre>
</div>

          <!-- KRNL Api -->
          <h1 id="krnlapi" class="headertext" align="center">Krnl API</h1><hr size="1" noshade="" color="#282828">
          <p class="desc">This is the documentation for the official Krnl API and how to use it. <br>The Krnl DLL is only designed for the official version of Roblox from their own site. Krnl will NOT inject into Roblox from the Microsoft Store, Linux or MacOs. <br><br>The API utilizes .NET Framework 4.8 (C#) <br><br> You can get the API <a style="color: rgb(100, 100, 200);" href="https://k-storage.com/bootstrapper/files/KrnlAPI.dll">here</a></p>

          <h1 id="howtouse" class="headertext" align="center">Using the API</h1>
          <h3 id="krnlapiclass">KrnlApi - class</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;"> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span> krnlApi = <span class="hljs-keyword" style="color: rgb(204, 153, 204);">new</span> <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>(); </pre>
          <p class="compactDesc">This is the main class of the API which is used to access every function of the API. Create a new instance of this class to start using the API</p>

          <hr size="1" noshade="" color="#282828">

          <h3 id="initializeapi">Initialize</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">void</span>&gt; <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.Initialize(); </pre>
          <p class="compactDesc">This method will set up the API and install all necessary files such as the DLL and only needs to be called one time. This method may cause a tiny bit of lag and should optimally be called when the application starts up. If lag is an issue, the API can be called through a thread.</p>

          <hr size="1" noshade="" color="#282828">

          <h3 id="injectapi">Inject</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">void</span>&gt; <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.Inject(); </pre>
          <p class="compactDesc">This method will inject the DLL into the active Roblox instance - keep in mind that the user has to go through the key system on their computer to gain unrestricted access to Krnl and the API.</p>

          <hr size="1" noshade="" color="#282828">

          <h3 id="executeapi">Execute</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">bool</span>&gt; <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.Execute(<span class="hljs-function">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">string</span>&gt; <span class="hljs-title" style="color: rgb(129, 162, 190);">script</span>); </span></pre>
          <p class="compactDesc">This method will execute the given script through the injected DLL. This will return true if the script has successfully been executed and false if there was a problem executing the script</p>

          <hr size="1" noshade="" color="#282828">

          <h3 id="setframerate">SetFrameRate</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">void</span>&gt; <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.SetFrameRate(<span class="hljs-function">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">int</span>&gt; <span class="hljs-title" style="color: rgb(129, 162, 190);">frameRate</span>); </span></pre>
          <p class="compactDesc">Sets the framerate of the active Roblox instance(s) to the desired value</p>

          <hr size="1" noshade="" color="#282828">

          <h3 id="isinjectedapi">IsInjected</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">bool</span>&gt; <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.IsInjected(); </pre>
          <p class="compactDesc">This method will check if the Krnl DLL has been injected</p>

          <hr size="1" noshade="" color="#282828">

          <h3 id="isinitializedapi">IsInitialized</h3>
          <pre class="hljs" style="display: block; overflow-x: auto; background: rgb(29, 31, 33); color: rgb(197, 200, 198); padding: 0.5em;">&lt;<span class="hljs-keyword" style="color: rgb(178, 148, 187);">bool</span>&gt; <span class="hljs-keyword" style="color: rgb(222, 147, 95);">KrnlApi</span>.IsInitialized(); </pre>
          <p class="compactDesc">This method will check if the API has been initialized</p>
        </div>
      </div>
    </div>
    <!-- Footer -->
    <hr style="margin-top:600px;" size="1" noshade="" color="#282828">
    <div class="fatfuck">
      <p style="padding-bottom: 10px;" align="center">Copyright © Krnl 2022</p>
    </div>
  </section>
