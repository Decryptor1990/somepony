<script>

  const APP_NAME = import.meta.env.VITE_APP_NAME;
  const APP_URL = import.meta.env.VITE_APP_URL;
  const APP_DOMAIN = import.meta.env.VITE_APP_DOMAIN;

  const URL_X = "#";
  const URL_TELEGRAM = "https://t.me/solar_ai_official";
</script>

<svelte:head>
	<title>{APP_NAME}</title>
	<meta name="description" content="{APP_NAME} :: an autonomous crypto investment AI service" />
  <meta name="twitter:card" content="summary">
	<meta name="twitter:title" content="{APP_NAME}">
	<meta name="twitter:description" content="{APP_NAME} :: an autonomous crypto investment AI service">
	<meta name="twitter:image" content="{APP_URL}/favicon/apple-touch-icon-152x152.png">
	<meta name="twitter:url" content={APP_URL}>
</svelte:head>

<header class="w-full"></header>
<section class="section mb-12 md:mb-24 relative">
  <div class="section-inner flex flex-col md:flex-row items-center md:h-[600px]">
    <div class="relative z-[2] w-full md:w-1/2 px-6 md:px-0 py-10 md:py-0 text-center md:text-left">
      <h1 class="h1 text-5xl md:text-7xl font-semibold mb-6 md:mb-8">
        {APP_NAME}
      </h1>
      <div class="mb-6 md:mb-8">
        <p class="text-lg md:text-xl text-slate-300">
          An autonomous <span class="font-semibold text-amber-300 max-md:block">crypto investment AI service</span>
        </p>
        <p class="text-lg md:text-xl text-slate-300">
          It's here to change the game rules
        </p>
      </div>

      <div class="flex justify-center md:justify-start">
        <a href="#details" class="btn btn--theme-yellow uppercase">
          Subscribe
        </a>
      </div>
    </div>
  </div>

  <img src="/img/bg-hero-2.jpg" alt="" class="absolute z-[1] top-0 right-0 h-full pointer-events-none max-md:opacity-50">
  <div class="absolute z-[2] left-[5%] md:left-[10%] bottom-0 w-[90%] md:w-[80%] h-px bg-gradient-to-r from-transparent via-amber-800 to-transparent"></div>
</section>

<section class="section mb-16 md:mb-24">
  <div class="section-inner px-6 md:px-0">
    <header 
      class="flex flex-col items-center justify-center mb-6"
      id="details"
    >
      <h2 class="h2 font-semibold text-2xl md:text-3xl">
        Base {APP_NAME} principles
      </h2>
      <p class="text-base text-center md:text-left md:text-lg text-gray-300">
        The {APP_NAME} model is constantly being trained on arrays of data and is evolving
      </p>
    </header>
    
    <div class="grid grid-cols-1 md:grid-cols-3 gap-x-8 gap-y-6">
      <div class="flex flex-row md:flex-col items-center">
        <figure class="flex flex-shrink-0 w-20 max-md:mr-4 md:w-auto max-w-40">
          <img src="/img/low-risk.png" alt="Low risk" class="saturate-50" />
        </figure>
        <div class="text-left md:text-center">
          <h3 class="h3 text-xl md:text-2xl font-semibold mb-1 md:mb-3">
            Low risk strategies
          </h3>
          <p class="text-sm md:text-base text-gray-300">
            Only safe trading strategies are used by {APP_NAME} to maximize efficiency without high risks for our clients
          </p>
        </div>
      </div>

      <div class="flex flex-row md:flex-col items-center">
        <figure class="flex flex-shrink-0 w-20 max-md:mr-4 md:w-auto max-w-40">
          <img src="/img/hype.png" alt="hype" class="saturate-50" />
        </figure>
        <div class="text-left md:text-center">
          <h3 class="h3 text-xl md:text-2xl font-semibold mb-1 md:mb-3">
            Hype data analysis
          </h3>
          <p class="text-sm md:text-base text-gray-300">
            A module for analyzing information events in social networks and the news sphere, as one of the main methods for predicting possible benefits
          </p>
        </div>
      </div>

      <div class="flex flex-row md:flex-col items-center">
        <figure class="flex flex-shrink-0 w-20 max-md:mr-4 md:w-auto max-w-40">
          <img src="/img/altcoin.png" alt="Altcoins" class="saturate-50" />
        </figure>
        <div class="text-left md:text-center">
          <h3 class="h3 text-xl md:text-2xl font-semibold mb-1 md:mb-3">
            Altcoin trading
          </h3>
          <p class="text-sm md:text-base text-gray-300">
            Trading on altcoins is the most marginal way of trading in the crypto industry.
            The {APP_NAME} automatically selects only reliable altcoins.
          </p>
        </div>
      </div>

    </div>
  </div>
</section>

<section class="section mb-16 md:mb-24">
  <div class="section-inner px-6 md:px-0 pb-10 md:pb-0 relative flex items-center">
    <header>
      <h2 class="h2 font-semibold text-2xl md:text-3xl md:flex  md:items-end md:gap-2">
        Guaranteed income 
        
        <div class="block md:inline-block">
          <span class="text-amber-300">up to 30%</span>
          <span class="text-base text-center md:text-left md:text-lg text-gray-300 md:pl-2">
            per month
          </span>
        </div>

      </h2>
      <p class="text-base text-center md:text-left md:text-lg text-gray-400">
        Trading samples will be published soon
      </p>
    </header>

    <div class="absolute max-md:bottom-0 max-md:left-6 md:right-0 flex items-center gap-x-1 md:gap-x-2">
      {#each Array(35) as _, idx}
        <!-- <div class="h-[{10*(idx+1)}px] w-2 bg-lime-400"></div> -->
        <div 
          class="w-1.5 md:w-1 h-6 md:h-10 bg-green-500 rounded-sm" 
          style="opacity: {0.03*(idx+1)};"
        ></div>
      {/each}
    </div>

  </div>
</section>




<!-- Investors -->
<section class="section mb-14 md:mb-24 relative z-[2]">
  <div class="section-inner px-6 md:px-0">
    <header class="flex flex-col justify-center mb-4 md:mb-6">
      <h2 class="h2 font-semibold text-3xl">
        Main investors
      </h2>
    </header>

    <div class="investor-list">
      <div class="investor-item">
        <img 
          src="/investors/paradigm.png" 
          alt="Paradigm" 
          class="investor-item--img" 
        />
        <p>
          Paradigm
        </p>
      </div>

      <div class="investor-item">
        <img 
          src="/investors/sequoia.png" 
          alt="Sequoia Capital"
          class="investor-item--img" 
        />
        <p>
          Sequoia Capital
        </p>
      </div>

      <div class="investor-item">
        <img 
          src="/investors/circle.png" 
          alt="Circle" 
          class="investor-item--img" 
        />
        <p>
          Circle
        </p>
      </div>

      <div class="investor-item">
        <img 
          src="/investors/consen_sys.png" 
          alt="ConsenSys" 
          class="investor-item--img" 
        />
        <p>
          ConsenSys
        </p>
      </div>
      <div class="investor-item">
        <img 
          src="/investors/variant.png" 
          alt="Variant" 
          class="investor-item--img" 
        />
        <p>
          Variant
        </p>
      </div>
    </div>
  </div>
</section>

<!-- Social media -->
<section class="section mb-14 md:mb-24 relative z-[2]">
  <div class="section-inner px-6 md:px-0">
    <header class="flex flex-col justify-center mb-4 md:mb-6">
      <h2 class="h2 font-semibold text-3xl">
        Stay tunned
      </h2>
      <p class="text-lg text-gray-300">
        Follow the {APP_NAME} team and stay tunned
      </p>
    </header>

    <div class="flex flex-col md:flex-row gap-8">
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
          <h5 class="text-lg leading-5 font-bold">
            {APP_NAME}
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
            {APP_NAME}
          </h5>
          <p class="text-base">
            on Telegram
          </p>
        </div>
      </a>
    </div>
  </div>
</section>

<footer class="section min-h-20 md:h-24 relative flex justify-center">
  <div class="section-inner pb-6 px-6 md:px-0 text-xs text-gray-400 flex flex-col gap-y-1">
    <p class="select-none">
      Location: 38, Beach Road, Singapore 189767, Floor 9 · South Beach Avenue, LLC {APP_NAME} inc
    </p>
    <p class="select-none">
      Contacts: +6566725722 | support@{APP_DOMAIN}
    </p>
    <p class="select-none">
      The {APP_NAME} serivce is the intellectual property of LLC {APP_NAME} inc.
    </p>
  </div>

  <div class="hero-glow -bottom-1 !h-0 !w-28 opacity-50">
  </div>
</footer>