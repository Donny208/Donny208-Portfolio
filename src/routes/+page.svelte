<script lang="ts">
    import Welcome from "$lib/components/cards/Welcome.svelte";
    import AboutMe from "$lib/components/cards/AboutMe.svelte";
    import Contact from "$lib/components/cards/Contact.svelte";
    import TimeZone from "$lib/components/cards/TimeZone.svelte";
    import CurrentProject from "$lib/components/cards/CurrentProject.svelte";
    import UpTo from "$lib/components/cards/UpTo.svelte";
    import ProjectBanner from "$lib/components/cards/ProjectBanner.svelte";
    import ProjectCard from "$lib/components/cards/ProjectCard.svelte";
    import Copyright from "$lib/components/cards/Copyright.svelte";
</script>

<div class="flex flex-row h-full justify-center">
    <div class="grid grid-cols-4 grid-rows-9 gap-1 w-full min-h-screen p-4">
        <div class="p-2 col-span-3 row-span-4">
            <Welcome/>
        </div>
        <div class="p-2 row-span-8">
            <AboutMe/>
        </div>
        <div class="p-2 row-span-5">
            <Contact/>
        </div>
        <div class="p-2 col-span-1 row-span-1">
            <TimeZone/>
        </div>
        <div class="p-2 row-span-3 col-span-1">
            <UpTo/>
        </div>
        <div class="p-2 row-span-2">
            <CurrentProject/>
        </div>
        <div class="p-2 col-span-2 row-span-1">
            <ProjectBanner/>
        </div>
        <div class="p-2">
            <ProjectCard
                    name="CareForMyPlant"
                    skills={["Python", "Embedded Systems"]}
                    imageURL="/img/careformyplant.jpg"
                    projectURL="https://github.com/Donny208/CareForMyPlant"
            />
        </div>
        <div class="p-2">
            <ProjectCard
                    name="HardwareScrape"
                    skills={["Rust", "PostgreSQL", "Docker"]}
                    imageURL="/img/hardwarescrape.png"
                    projectURL="https://github.com/Donny208/Hardware-Scrape"
            />
        </div>
        <div class="p-2">
            <Copyright/>
        </div>
    </div>
</div>