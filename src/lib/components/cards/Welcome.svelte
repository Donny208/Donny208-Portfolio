<script lang="ts">
    import Icon from '@iconify/svelte';
    import * as Card from "$lib/components/ui/card";
    import {EMAIL, GITHUB_URL, LINKEDIN_URL} from "$lib/config"
</script>

<Card.Root class="h-full">
    <Card.Header>
        <Card.Title>Welcome</Card.Title>
    </Card.Header>
    <Card.Content class="flex flex-row h-full justify-evenly">
        <div class="flex flex-col max-h-full w-2/3 justify-between">
            <div class="max-h-1/2 space-y-3 text-[100%]">
                <p>I'm <b>Donovan Wright</b>, a software developer with over four years of professional experience and more than ten years of coding expertise. I specialize in full-stack development, bringing a balanced approach to both front-end and back-end solutions.</p>
                <p>Whether you have a project in mind or simply want to connect, feel free to reach out!</p>
            </div>
            <div class="h-1/2 w-full flex flex-row justify-evenly items-center gap-2　mb-5">
                <a href={GITHUB_URL} target="_blank">
                    <div class="rounded-lg w-12 h-12 xl:w-20 xl:h-20 bg-purple-300 flex items-center justify-center">
                        <Icon icon="mdi:github" class="size-[50%]"/>
                    </div>
                </a>
                <a href={LINKEDIN_URL} target="_blank">
                    <div class="rounded-lg w-12 h-12 xl:w-20 xl:h-20 bg-purple-300 flex items-center justify-center">
                        <Icon icon="mdi:linkedin" class="size-[50%]"/>
                    </div>
                </a>
                <a href={`mailto:${EMAIL}`}>
                    <div class="rounded-lg w-12 h-12 xl:w-20 xl:h-20 bg-purple-300 flex items-center justify-center">
                        <Icon icon="mdi:email" class="size-[50%]" />
                    </div>
                </a>
            </div>
        </div>
        <div class="flex flex-col justify-end max-h-full w-1/3 -mt-5">
            <img src="/img/largeMe.png" alt="Emoji of Donovan" class="object-contain h-[65%] w-[65%]">
        </div>
    </Card.Content>
</Card.Root>