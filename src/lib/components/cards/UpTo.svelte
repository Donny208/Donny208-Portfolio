<script lang="ts">
    import * as Card from "$lib/components/ui/card";
</script>

<Card.Root class="h-full">
    <Card.Header>
        <Card.Title>Work Overview</Card.Title>
        <Card.Description>Most recent experience on the top</Card.Description>
    </Card.Header>
    <Card.Content>
        <div>
            <ul>
                <li>
                    <div class="flex flex-col">
                        <div class="flex flex-row justify-between">
                            <p class="text-sm font-bold">Software Developer</p>
                            <p class="text-xs italic">Data Fleet</p>
                        </div>
                        <div class="flex flex-row justify-between text-xs">
                            <p>Python, React, JavaScript, Node.js, Docker, Git, PostgreSQL, Firebase, GCP, etc.</p>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="flex flex-col border-t border-gray-500">
                        <div class="flex flex-row justify-between">
                            <p class="text-sm font-bold">Software Engineer</p>
                            <p class="text-xs italic">Micron Technology</p>
                        </div>
                        <div class="flex flex-row justify-between text-xs">
                            <p>C#, ASP.NET, Angular, TypeScript, Git, SQL, Docker, Azure Cloud Services, etc.</p>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </Card.Content>
</Card.Root>