<script>
    import alternativeDownloads from '@assets/data/miscdownloads.json'
    const tabsmisc = alternativeDownloads.Providers
    let activeTab = 0
</script>

<div>
    <div class="flex flex-wrap gap-1 text-2xl py-4 px-3 bg-black/60">
        {#each tabsmisc as tab, i}
            <button class="flex-auto text-center text-xl mx-auto rounded px-5 py-2.5 font-bold cursor-pointer transition duration-200 ease-in-out hover:bg-white/50" 
                class:bg-white={i === activeTab} 
                class:text-black={i === activeTab}
                class:text-white={i !== activeTab}
                on:keypress={() => activeTab = i}
                on:click={() => activeTab = i}>
                {tab.name}
    </button>
        {/each}
    </div>

    <div class="flex justify-center items-center gap-4 px-5 py-5 bg-white/60">
        {#each tabsmisc[activeTab].links as link}
        <a href={link.link}
        class="flex-auto rounded text-center transition focus-visible:ring-2 ring-offset-2 ring-gray-200 px-5 py-2.5 button-glow font-semibold bg-white text-black flex gap-1 items-center justify-center">
        {link.name}
        </a>
        {/each}
    </div>
</div>

<style>
    .button-glow{
    position: relative;
    z-index: 0;
    }
    .button-glow:before{
    content: '';
    background: linear-gradient(45deg, #ff0000, #ff7300, #fffb00, #48ff00, #00ffd5, #002bff, #7a00ff, #ff00c8, #ff0000);
    position: absolute;
    top: 0px;
    left: 0px;
    background-size: 600%;
    z-index: -1;
    width: 100%;
    height: 100%;
    animation: glowing 20s linear infinite;
    backdrop-filter: blur(10px);
    filter: blur(2px);
    opacity: 0;
    transition: opacity .3s ease-in-out;
    border-radius: 0.25rem;
    }
    .button-glow:hover:before {
    opacity: 1;
    }
    
    @keyframes glowing {
      0% { background-position: 0 0; }
      50% { background-position: 400% 0%; }
      100% { background-position: 0 0; }
    }
    </style>
  