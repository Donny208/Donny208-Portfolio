<script lang="ts">
    import * as Card from "$lib/components/ui/card";
    import {EMAIL, GITHUB_URL, LINKEDIN_URL} from "$lib/config"
</script>

<Card.Root class="h-full">
    <Card.Header>
        <Card.Title>Contact</Card.Title>
        <Card.Description>Let's get in touch!</Card.Description>
    </Card.Header>
    <Card.Content>
        <div class="flex flex-col h-full justify-evenly space-y-[30%] text-[100%]">
            <div>
                <h1 class="font-bold">Contact Details</h1>
                <a href={`mailto:${EMAIL}`}>
                    <p class="italic">{EMAIL}</p>
                </a>
            </div>
            <div>
                <h1 class="font-bold">Social Media</h1>
                <a href={GITHUB_URL} target="_blank">
                    <p>Github</p>
                </a>
                <a href={LINKEDIN_URL} target="_blank">
                    <p>LinkedIn</p>
                </a>
            </div>
        </div>
    </Card.Content>
</Card.Root>