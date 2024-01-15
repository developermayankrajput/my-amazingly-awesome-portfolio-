<script>
    export let y;
    let tabs = [
        {name: "Skills",link: "#introduction"},
        { name: "Projects", link: "#projects" },
        { name: "Resume", link: "#" },
        { name: "About Me", link: "#about" },
    ];
</script>

<header
    class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid " +
        (y > 0
            ? " py-4 bg-slate-950 border-cyan-950"
            : " py-6 bg-transparent border-transparent")}
>
    <h1 class="font-medium text-xl">
        <b class="font-bold poppins">Mayank</b> Rajput
    </h1>
    <div class="sm:flex ml-auto pr-4 items-center gap-4 hidden">
        {#each tabs as tab, index}
            <a href={tab.link} class="duration-200 hover:text-cyan-400">
                <p>{tab.name}</p>
            </a>
        {/each}
    </div>
    <a
    href="#getintouch"
        class="blueShadow realtive overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950"
    >
        <div
            class="absolute top-0 h-full bg-cyan-900 opacity-20 group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative z-9 group-hover:text-cyan-400">Get in touch</h4>
    </a>
</header>
