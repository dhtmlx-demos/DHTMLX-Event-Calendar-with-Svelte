<script>
    import { onMount } from "svelte";
    
    import { EventCalendar } from "@dhx/trial-eventcalendar";
    import "@dhx/trial-eventcalendar/dist/event-calendar.css";
    
    export let events;
    export let date;

    let container;
    onMount(() => {
        new EventCalendar(container, {
            events, date
        })
    });
</script>

<div bind:this={container} style="width: 100%; height: 100%;"></div>

