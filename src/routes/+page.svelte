<script>
 let tempData = [];

onMount(async () => {

    const res = await fetch('temperatures.csv'); 

    const csv = await res.text();

    tempData = d3.csvParse(csv, d3.autoType)

    console.log(tempData);

});

</script>


<h1>Welcome to the page</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
