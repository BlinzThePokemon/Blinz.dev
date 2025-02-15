<script>
    import "../app.css";
    import { page } from "$app/state";
    let { children } = $props();
    let navBarItems = [
        { name: "Home", id: "/" },
        { name: "Projects", id: "/Projects" },
        { name: "Links", id: "/Links" },
        { name: "Posts", id: "/Posts" },
    ];
</script>

<nav class=" shadow-md top-0 fixed w-full backdrop-blur-lg">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="flex h-16 items-center justify-center">
            <div class="hidden space-x-4 sm:flex fixed">
                {#each navBarItems as item}
                    {@const path = page.url.pathname.split("/")[1]}
                    {@const selected = path === item.id.split("/")[1]}

                    <a
                        class:bg-gray-900={selected}
                        class:text-white={selected}
                        href={item.id}
                        class="rounded-md px-3 py-2 text-md font-medium transition duration-300 ease-in-out hover:bg-gray-500 hover:text-white active:bg-gray-900 active:text-white"
                        >{item.name}</a
                    >
                {/each}
            </div>
            <i
                class="fa-solid fa-gear ml-[1750px] text-3xl transition-all delay-100 duration-300 ease-in-out hover:text-4xl fa-spin">
            </i>
        </div>
    </div>
</nav>

{@render children()}
