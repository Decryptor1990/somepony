<script>
  import { onMount } from "svelte";

  const SITE_URL = "https://tumpony.fun";
  const TOKEN = "Trumpony";
  const URL_X = "https://x.com/TRUMPonyFUN";
  const URL_TELEGRAM = "https://t.me/trumponyfun";
  const URL_PUMPFUN = "https://pump.fun/coin/F5dPeLsEt1gksYgpXG8XRBNzaaZ7RVEbVnSmpa3Gpump";
  const URL_TEAM = "https://t.me/h4xedby";

  let show = $state(false);

  onMount(() => {
    setTimeout(() => {
      show = true;
    }, 350)
  })
</script>

<svelte:head>
	<title>{TOKEN} :: new hero meme token</title>
	<meta name="description" content="{TOKEN} :: new awesome hero meme token. It is here to make Meme Coins GREAT AGAIN!" />
  <meta name="twitter:card" content="summary">
	<meta name="twitter:title" content="{TOKEN} :: new hero meme token">
	<meta name="twitter:description" content="{TOKEN} :: new awsome hero meme token. It is here to make Meme Coins GREAT AGAIN!">
	<meta name="twitter:image" content="{SITE_URL}/trumpony-token.png">
	<meta name="twitter:url" content={SITE_URL}>
</svelte:head>

<header class="w-full"></header>
<section class="section mb-12 md:mb-24">
  <div class="section-inner flex flex-col md:flex-row items-center md:h-[664px]">
    <div class="w-full md:w-1/2 px-6 md:px-0 py-6 md:py-0 text-center md:text-left">
      <p class="text-xl text-slate-400">
        Say #hello to
      </p>
      <h1 class="h1 text-5xl md:text-7xl font-semibold mb-4 md:mb-2">
        {TOKEN}
      </h1>
      <p class="text-lg md:text-xl text-slate-300 md:mb-8">
        a new <span class="font-semibold text-amber-300">hero meme token</span>!
      </p>
      <p class="text-lg md:text-xl text-slate-300 mb-4 md:mb-8">
        It's here to make Meme Coins<br>
        <span class="text-xl md:text-2xl font-semibold">
          GREATE AGAIN!
        </span>
      </p>

      <div class="flex justify-center md:justify-start">
        <a href="#details" class="btn btn--theme-yellow uppercase">
          Get started
        </a>
      </div>
    </div>
    <div class="w-full md:w-1/2 flex items-center justify-center relative h-80 md:h-auto"> 
      <div class="hero-glow"></div>
      <img 
        src="/trumpony-token--no-bg.png" 
        alt="trumpony-token" 
        class="h-80 md:h-auto max-w-[500px] relative z-[2]  transition-all duration-[1600ms]" 
        class:translate-y-28={!show}
        class:scale-50={!show}
        class:opacity-0={!show}
      />
    </div>
  </div>
</section>

<section class="section mb-16 md:mb-24">
  <div class="section-inner px-6 md:px-0">
    <header 
      class="flex flex-col items-center justify-center mb-4"
      id="details"
    >
      <h2 class="h2 font-semibold text-3xl">
        {TOKEN} main values
      </h2>
      <p class="text-base md:text-lg text-slate-400">
        You've been waiting for a powerful and independent meme coin on a wave of popularity, and it's here
      </p>
    </header>
    
    <div class="grid grid-cols-1 md:grid-cols-3 gap-x-6 gap-y-6">
      <div class="flex flex-row md:flex-col items-center">
        <figure class="flex flex-shrink-0 w-28 md:w-auto max-w-56">
          <img src="fun.png" alt="fun" />
        </figure>
        <div class="text-left md:text-center">
          <h3 class="h3 text-2xl font-semibold">
            Fun
          </h3>
          <p class="text-base md:text-lg text-gray-300">
            Be a part of crypto society and create a new trend and fun <span class="font-semibold text-amber-200">{TOKEN}</span> token with us!
          </p>
        </div>
      </div>

      <div class="flex flex-row md:flex-col items-center">
        <figure class="flex flex-shrink-0 w-28 md:w-auto max-w-56">
          <img src="freedom.png" alt="freedom" />
        </figure>
        <div class="text-left md:text-center">
          <h3 class="h3 text-2xl font-semibold">
            Freedom
          </h3>
          <p class="text-base md:text-lg text-gray-300">
            Be one of the first <span class="font-semibold text-amber-200">{TOKEN}</span> token owner and multiply your profit X5 or X10 or even X100!
          </p>
        </div>
      </div>

      <div class="flex flex-row md:flex-col items-center">
        <figure class="flex flex-shrink-0 w-28 md:w-auto max-w-56">
          <img src="hype.png" alt="hype" />
        </figure>
        <div class="text-left md:text-center">
          <h3 class="h3 text-2xl font-semibold">
            Hype
          </h3>
          <p class="text-base md:text-lg text-gray-300">
            Let's push it up with a new President! Make Meme Coins Great Again and pump <span class="font-semibold text-amber-200">{TOKEN}</span> up the hype!
          </p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="section mb-14 md:mb-24 relative z-[2]">
  <div class="section-inner px-6 md:px-0">
    <header class="flex flex-col justify-center mb-4 md:mb-6">
      <h2 class="h2 font-semibold text-3xl">
        Stay tunned
      </h2>
      <p class="text-lg text-gray-300">
        Follow  the {TOKEN} token team and stay tunned
      </p>
    </header>

    <div class="flex flex-col md:flex-row gap-8">
      <a 
        href={URL_PUMPFUN}
        target="_blank" 
        class="social-link"
      >
        <img 
          src="/social/pumpfun.png" 
          alt="pumpfun" 
          class="size-10"
        />
        <div class="flex flex-col text-amber-400 ">
          <h5 class="text-lg leading-5 font-bold ">
            {TOKEN} token
          </h5>
          <p class="text-base">
            on Pump.fun
          </p>
        </div>
      </a>

      <a 
        href={URL_X}
        target="_blank"
        class="social-link"
      >
        <img 
          src="/social/x.png" 
          alt="pumpfun" 
          class="size-10"
        />
        <div class="flex flex-col text-amber-400 ">
          <h5 class="text-lg leading-5 font-bold ">
            {TOKEN} token
          </h5>
          <p class="text-base">
            on X.com
          </p>
        </div>
      </a>

      <a 
        href={URL_TELEGRAM}
        target="_blank"
        class="social-link"
      >
        <img 
          src="/social/telegram.png" 
          alt="pumpfun" 
          class="size-10"
        />
        <div class="flex flex-col text-amber-400 ">
          <h5 class="text-lg leading-5 font-bold ">
            {TOKEN} token
          </h5>
          <p class="text-base">
            on Telegram
          </p>
        </div>
      </a>
    </div>
  </div>
</section>

<footer class="section h-20 md:h-24 relative flex justify-center">
  <div>
    <a 
      href={URL_TEAM} 
      target="_blank" 
      class="text-gray-600 рh-fit text-sm border-b border-gray-700 hover:text-sky-600 hover:border-sky-700 transition-colors"
    >
      <span class="font-bold">DC</span> meme-maker team
    </a>
  </div>

  <div class="hero-glow -bottom-1 !h-0 !w-28 opacity-50">
  </div>
</footer>