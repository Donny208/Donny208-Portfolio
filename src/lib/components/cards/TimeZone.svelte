<script lang="ts">
    import {onMount} from "svelte";

    let time: string;

    /**
     * Returns the current time in mountain time in the format hh:mm:ss <tz>
     */
    const getCurrentMountainTime = (): string  => {
        return new Date().toLocaleString("en-US", {
            timeZone: "America/Denver",
            hour: "2-digit",
            minute: "2-digit",
            second: "2-digit",
            hour12: true,
            timeZoneName: "short",
        });
    }

    onMount(() => {
        //Fetch the initial time & update every second
        time = getCurrentMountainTime();
        setInterval(() => {
            time = getCurrentMountainTime();
        }, 1000);
    });
</script>

<div class="bg-purple-400 min-h-full min-w-full rounded-lg text-lg flex items-center justify-center">
    <p>{time}</p>
</div>