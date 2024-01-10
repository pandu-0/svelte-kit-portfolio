<script>
    export let y;

    // Header tabs
    // using #id will map to that element with that specific id
    // I use this to auto scroll
    let tabs = [
        { name: 'Projects', link: '#projects' },
        { name: 'About me', link: '#about' },
        { name: 'Contact', link: '#contact' }
    ]
</script>

<header
    class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid " +
        (y > 0
            ? " py-4 bg-slate-950 border-violet-950"
            : " py-6 bg-transparent border-transparent")}
>
    <!-- Pandu header -->
    <a href="https://www.youtube.com/watch?v=wh9QLjk3M2k&pp=ygUXY2h1cGkgY2h1cGkgY2hhcGEgY2hhcGE%3D" target="_blank">
        <h1 class="font-medium">
            <div class="duration-200 hover:text-orange-400">
                <b style="font-size: large;text-shadow: 2px 2px 3px grey;" class="font-bold poppins">
                    Pandu
                </b>
            <div/>
        </h1>
    </a>
    <!-- Projects, About me, and Contact Header Tabs -->
   <div style="text-shadow: 2px 2px 3px grey;" class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab, index}

        <a style="font-size: large;"
            href={tab.link} 
            class="duration-200 hover:text-violet-400"
            target="_self"
        >
            <p>{tab.name}</p>
        </a>
        {/each}
   </div>

   <!-- Linkedin Link -->
   <a style="box-shadow: 2px 2px 3px grey;text-shadow: 3px 3px 3px lightgrey;"
        href="https://www.linkedin.com/in/manmohanbabu-rupanagudi-639241249/"
        target="_blank"
        class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white 
        text-slate-950">
        <div
            class="absolute top-0 right-full w-full h-full bg-violet-400 
            opacity-20 group-hover:translate-x-full z-0 duration-200"
        />
        <!--Header Get in touch button -->
        <h4 style="font-size: medium;" class="relative z-9">Connect &uarr;</h4>
    </a>
</header>