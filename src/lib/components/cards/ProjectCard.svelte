<script lang="ts">
    import Icon from '@iconify/svelte';
    export let name: string;
    export let skills: string[];
    export let imageURL: string;
    export let projectURL: string;
</script>

<a href={projectURL} target="_blank">
    <div
            style={`background-image: linear-gradient(to right, rgb(192, 132, 252) 0%, rgba(255, 255, 255, 0)), url(${imageURL});`}
            class="min-h-full min-w-full rounded-lg flex flex-row items-center justify-between p-2 bg-cover bg-center"
    >
        <div>
            <h1 class="font-bold">{name}</h1>
            <p class="text-xs">{skills.join(', ')}</p>
        </div>
        <Icon icon="mdi-light:fullscreen" class="size-7"/>
    </div>
</a>
