<head>
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.13.1/css/all.css">
</head>
<script>
import { fade, fly } from 'svelte/transition';

	let barWidth = 0;
	let progress;
  const addColor = () => barWidth += 5;
	
	const randomTime = () => 1  

  progress = setInterval(addColor, randomTime());		


  if (barWidth > 600) {
    document.getElementById("card").style.height = "600px"

  }
</script>
{#if barWidth < 600}

<div id="myProgress">
  <h1>Loading...</h1>
  <div id="myBar" style="width: {barWidth}px; color:grey;"></div>



</div>
{/if}
<main>

  
  {#if barWidth > 600}

  
  <div id="card" transition:fly class="card" >
   <h1 class="name">
      ui#0873 
</h1>
    <div class="quote-holder">
    <p class="quote">fuck u 💬</p></div>
<ul class="langs">
      <li>

      <li>
        <i style="font-size: 30px; color: rgba(71, 167, 255, 1);" class="fab fa-css3"></i>
        </li>
      <li>
        <i style="font-size: 30px; color: rgba(71, 167, 255, 1);" class="fab fa-html5"></i>
      
      </li>
      <li>
        <i style="font-size: 30px; color: rgba(71, 167, 255, 1);" class="fab fa-python"></i>
      </li>
      <li>
        <i style="font-size: 30px; color: rgba(71, 167, 255, 1);" class="fab fa-js"></i>
      </li>

    
    </ul>
    <div class="bd"> </div>


    <ul class="socials">
<li>
  <a href="https://ui_btc.t.me">
  <i style="font-size: 30px; color: rgba(71, 167, 255, 1);" class="fab fa-telegram"></i>
  </a>
</li>
<li>
  <a href="https://tiktok.com/@floor">
  <i class="fab fa-tiktok" style="font-size: 30px; color: rgba(71, 167, 255, 1);"></i>
  </a>
</li>
<li>
  <a href="https://discord.gg/4dJPuEqT">
  <i class="fab fa-discord" style="font-size: 30px; color: rgba(71, 167, 255, 1);"></i>
  </a>
</li>
<li>
  <a href="https://github.com/uiisback">
  <i class="fab fa-github" style="font-size: 30px; color: rgba(71, 167, 255, 1);"></i>
  </a>
</li>
    </ul>
  </div>
  {/if}
</main>
