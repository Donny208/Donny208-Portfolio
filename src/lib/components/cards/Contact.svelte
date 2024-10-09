<script lang="ts">
    import * as Card from "$lib/components/ui/card";
</script>

<Card.Root class="h-full">
    <Card.Header>
        <Card.Title>Contact</Card.Title>
        <Card.Description>Let's get in touch!</Card.Description>
    </Card.Header>
    <Card.Content class="h-full">
        <div class="flex flex-col h-full justify-evenly">
            <div>
                <h1 class="font-bold">Contact Details</h1>
                <a href="mailto:new_email_here@gmail.com">
                    <p class="italic">new_email_here@gmail.com</p>
                </a>
            </div>
            <div>
                <h1 class="font-bold">Social Media</h1>
                <a href="https://github.com/Donny208" target="_blank">
                    <p>Github</p>
                </a>
                <a href="https://www.linkedin.com/in/dww/" target="_blank">
                    <p>LinkedIn</p>
                </a>
            </div>
        </div>
    </Card.Content>
</Card.Root>