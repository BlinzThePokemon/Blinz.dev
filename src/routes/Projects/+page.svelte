<script>
    import Projects from "../Components/projects.svelte";

    let ProjectsInfo = [
        { title: "Scratch Addons (Translation)", icon: "", text: "I am one of the Eng to Hin traslators of Scratch Addons; A collection of addons or kids' coding platoform - Scratch <br><br> You can check it out <a target='_blank' href='https://scratchaddons.com'>Here</a>"}
    ]
</script>
<p class="flex justify-center mt-20 font-bold text-6xl">My Projects</p>
<div class="flex justify-center mt-10">
    {#each ProjectsInfo as ProjectInfo}
        <div class="bg-gray-300 rounded-2xl w-4/5 h-48">
            <div class="inline-flex  text-3xl font-bold">
                <img src="{ProjectsInfo.icon}" alt="">
                 <p class="ml-5 mt-2">{ProjectInfo.title}</p>
            </div>
                <p class="text-lg ml-5">{@html ProjectInfo.text}</p>
        </div>
    {/each}
</div>

<style>
    ::selection {
    background: orange;
}
p :global{
    a{
        text-decoration: underline;
        transition: all 200ms;
        text-decoration-thickness: 2px;
    
    &:hover{
        font-size: larger;
    }
    }
}
</style>