<script>
  import Calendar from "./Calendar.svelte";
  import { getData } from "./data.js";
</script>

<Calendar events={getData()} date={new Date(2021, 5, 10)} />
